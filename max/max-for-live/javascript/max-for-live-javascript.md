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
