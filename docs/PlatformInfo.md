# PlatformInfo

Public metadata for one registered plugin (admin UI). Maps 1:1 from [`plugin_core::PluginInfo`] (same field shape as before).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**author** | **str** |  | 
**changelog** | [**List[ChangelogEntry]**](ChangelogEntry.md) |  | 
**config_field_names** | **List[str]** |  | 
**config_fields** | [**List[ConfigFieldInfo]**](ConfigFieldInfo.md) |  | 
**display_name** | **str** |  | 
**platform** | **str** |  | 
**pricing** | [**PluginPricing**](PluginPricing.md) |  | 
**supported_entities** | **List[str]** |  | 
**supports_export** | **bool** |  | 
**supports_import** | **bool** |  | 
**supports_oauth** | **bool** |  | 
**version** | **str** |  | 

## Example

```python
from simplebilly_api.models.platform_info import PlatformInfo

# TODO update the JSON string below
json = "{}"
# create an instance of PlatformInfo from a JSON string
platform_info_instance = PlatformInfo.from_json(json)
# print the JSON string representation of the object
print(PlatformInfo.to_json())

# convert the object into a dict
platform_info_dict = platform_info_instance.to_dict()
# create an instance of PlatformInfo from a dict
platform_info_from_dict = PlatformInfo.from_dict(platform_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


