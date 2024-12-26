# Max JavaScript LiveAPI

Create a LiveAPI object:

``` javascript
  var devicesPath = "live_set tracks " + id + " devices";
  var trackAPI = new LiveAPI();
```

Dump info about the object:

``` javascript
  post("deviceAPI.info = " + deviceAPI.info + "\n");
```

Getting values (properties and root level values):

``` javascript
  post("id = " + deviceAPI.id + "\n");
  post("name = " + deviceAPI.get("name") + "\n");
```
