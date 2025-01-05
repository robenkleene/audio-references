# Max for Live Javascript Snippets

## Device Name

``` javascript
  var deviceAPI = new LiveAPI("live_set tracks 0 devices 3");
  outlet(0, deviceAPI.get("name"));
```
