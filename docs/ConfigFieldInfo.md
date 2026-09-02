# ConfigFieldInfo

Owned, API-safe copy of a [`ConfigField`] for DTOs / OpenAPI ([`ConfigField`] borrows `&'static str`, which cannot round-trip `Deserialize`).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**kind** | [**ConfigFieldKind**](ConfigFieldKind.md) |  | 
**label** | **str** |  | 
**name** | **str** |  | 
**placeholder** | **str** |  | [optional] 
**required** | **bool** |  | 

## Example

```python
from simplebilly_api.models.config_field_info import ConfigFieldInfo

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigFieldInfo from a JSON string
config_field_info_instance = ConfigFieldInfo.from_json(json)
# print the JSON string representation of the object
print(ConfigFieldInfo.to_json())

# convert the object into a dict
config_field_info_dict = config_field_info_instance.to_dict()
# create an instance of ConfigFieldInfo from a dict
config_field_info_from_dict = ConfigFieldInfo.from_dict(config_field_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


