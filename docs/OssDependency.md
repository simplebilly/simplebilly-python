# OssDependency


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dependency_type** | **str** |  | 
**license** | **str** |  | [optional] 
**name** | **str** |  | 
**version** | **str** |  | 

## Example

```python
from simplebilly_api.models.oss_dependency import OssDependency

# TODO update the JSON string below
json = "{}"
# create an instance of OssDependency from a JSON string
oss_dependency_instance = OssDependency.from_json(json)
# print the JSON string representation of the object
print(OssDependency.to_json())

# convert the object into a dict
oss_dependency_dict = oss_dependency_instance.to_dict()
# create an instance of OssDependency from a dict
oss_dependency_from_dict = OssDependency.from_dict(oss_dependency_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


