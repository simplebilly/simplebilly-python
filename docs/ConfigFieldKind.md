# ConfigFieldKind


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**options** | **List[str]** |  | 

## Example

```python
from simplebilly_api.models.config_field_kind import ConfigFieldKind

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigFieldKind from a JSON string
config_field_kind_instance = ConfigFieldKind.from_json(json)
# print the JSON string representation of the object
print(ConfigFieldKind.to_json())

# convert the object into a dict
config_field_kind_dict = config_field_kind_instance.to_dict()
# create an instance of ConfigFieldKind from a dict
config_field_kind_from_dict = ConfigFieldKind.from_dict(config_field_kind_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


