# Max JavaScript Outlets

If the output of the outlet is printing `jsobject` followed by an address, it probably needs to be converted from an object `(post(typeof name + ": " + name + "\n");`) to a primitive (e.g., `String(deviceAPI.get("name"))`).

``` javascript
  for (var i = 0; i < children.length; i++) {
    var devicePath = devicesPath + " " + i;
    var deviceAPI = new LiveAPI(devicePath);
    devicesIDs.push(deviceAPI.id);
    deviceNames.push(String(deviceAPI.get("name")));
  }
  outlet(0, deviceNames);
```