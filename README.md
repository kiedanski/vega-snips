# Vega Snips
The useful collections of vega tips


# Debugging

## Create view element while rendering

```js
  var view = {};
  var spec = "name.vg.json";
  vegaEmbed('#vis', spec).then(function(result) {
    view = result.view;
  }).catch(console.error);
```
then use it to inspect your dataset

```js
// In the developer console
view.data('name')
```
