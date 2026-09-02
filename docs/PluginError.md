# PluginError


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bad_request** | **List[object]** |  | 
**not_found** | **List[object]** |  | 
**unauthorized** | **List[object]** |  | 
**internal_error** | **List[object]** |  | 
**database_error** | **List[object]** |  | 
**validation_error** | **List[object]** |  | 
**not_implemented** | **str** |  | 

## Example

```python
from simplebilly_api.models.plugin_error import PluginError

# TODO update the JSON string below
json = "{}"
# create an instance of PluginError from a JSON string
plugin_error_instance = PluginError.from_json(json)
# print the JSON string representation of the object
print(PluginError.to_json())

# convert the object into a dict
plugin_error_dict = plugin_error_instance.to_dict()
# create an instance of PluginError from a dict
plugin_error_from_dict = PluginError.from_dict(plugin_error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


