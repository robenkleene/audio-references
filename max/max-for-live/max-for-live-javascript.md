# Max for Live JavaScript

- When editing a JavaScript file in Max for Live, to save, just click the close button on the window and it'll prompt to save changes
- JavaScript files default to `1` inlet and `1` outlet

## Troubleshooting

- It seems like it's impossible to get Max for Live to cleanly reload external JavaScript via `require()`. The files will re-compile, but the old versions of the JavaScript will still be called. The only things that work are completely quitting Live and re-opening, or running the JavaScript in Max instead of Live.

## Life Cycle

A `function loadbang()` will be called along with patcher `loadbang`, but only if this is the default script (e.g., `js <script-name>`).

When a script is first loaded the global JavaScript is run. After that only the called functions are run.

This means with the following example:

``` javascript
var counter = 0;
post("counter = " + counter + "\n");

function bang() {
	counter++;
	post("bang counter = " + counter + "\n");
}
```

- `counter = 0` will be printed when the script is first compiled
- `counter = 1` will be printed when the script is first run
- Subsequently the counter will be incremented by `1` each time it's run

## Dict

- Strangely `setparse` with a an array (e.g., `d.setparse("key", '[ { "foo": "bar" } ]');`) doesn't seem to work

## Template

``` javascript
// Re-compile the file automatically when it changes
autowatch = 1;

// Inlets & Outlets
inlets = 3;
outlets = 3;

// Store input
var values = [0, 0, 0];

// `inlet` property reports the inlet number

// `msg_int()` is called when an int is received
function msg_int(value) {
  values[inlet] = value;
  outlet(inlet, "int " + value);
}

// `msg_float()` is called when a float is received
function msg_float(value) {
  values[inlet] = value;
  outlet(inlet, "float " + value);
}

// `bang()` is called when a bang is received
function bang() {
  // The string `"bang"` sends a bang out the outlet
  outlet(inlet, "bang");
}

// `list()` is called when a message starts with `list`
// Only messages that beginning with a number (e.g., `1, b, 3, d`) will call
// `list` (otherwise `anything` will be called).
function list(value) {
  // `value` is only the first argument
  // If the first parameter is a symbol, then it's treated as a function name
  post("value = " + value);
  // If the input is all numbers, `messagename` is `list`
  post("messagename = " + messagename);
  process_arguments(inlet, messagename, arguments, "list");
}

// `anything()` is called when there's no function match
function anything(value) {
  // `value` is only the first argument
  post("value = " + value);
  // If input starts `messagename` is the first symbol in a list
  // E.g., if `a b c` is passed in, it's `a`
  post("messagename = " + messagename);
  process_arguments(inlet, messagename, arguments, "anything");
}

function process_arguments(inlet, firstElement, arguments, prefix) {
  // In a called function, `messagename` is the name of the function that called this one (e.g., `anything` or `list`)
  // The `arguments` property can be numerically indexed like an `Array` but is not an instance of `Array`.
  // `arrayfromargs` converts to an actual array
  var arr = arrayfromargs(firstElement, arguments);
  outlet(inlet, prefix + " " + arr.join());
}

function log(obj) {
  // `post` logs to console
  post(JSON.stringify(obj));
}
```
