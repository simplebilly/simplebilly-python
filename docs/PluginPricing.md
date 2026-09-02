# PluginPricing

How a plugin is priced in the marketplace. Tagged on `type` so the same enum deserializes both the API DTO and the `plugin_marketplace.json` manifest (`{\"type\":\"free\"}` / `{\"type\":\"one_time\",\"price\":99.0}` / `{\"type\":\"recurring\",\"price_per_month\":19.9}`).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**price** | **float** |  | 
**price_per_month** | **float** |  | 

## Example

```python
from simplebilly_api.models.plugin_pricing import PluginPricing

# TODO update the JSON string below
json = "{}"
# create an instance of PluginPricing from a JSON string
plugin_pricing_instance = PluginPricing.from_json(json)
# print the JSON string representation of the object
print(PluginPricing.to_json())

# convert the object into a dict
plugin_pricing_dict = plugin_pricing_instance.to_dict()
# create an instance of PluginPricing from a dict
plugin_pricing_from_dict = PluginPricing.from_dict(plugin_pricing_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


