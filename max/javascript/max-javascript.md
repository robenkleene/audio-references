# Max JavaScript

- Examples are at `~/Library/Application Support/Cycling '74/Max 8/Examples/javascript/`
- ES5 is used as of Max 8

## Notes

- Max JavaScript does not support default parameters for functions

## Printing

``` javascript
function log(obj) {
  post(JSON.stringify(obj));
}
```

For a new line, just do a `post();` alone on its own line

## Dict

Max `Dict` doesn't support arrays of dictionaries, so you can do this:

``` javascript
d.set("foo", barDictArr);
```
