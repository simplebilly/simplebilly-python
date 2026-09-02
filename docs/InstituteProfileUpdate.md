# InstituteProfileUpdate

Partial update of the institute profile.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**institute_type** | **str** |  | [optional] 
**kapitalmarktorientiert** | **bool** |  | [optional] 

## Example

```python
from simplebilly_api.models.institute_profile_update import InstituteProfileUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of InstituteProfileUpdate from a JSON string
institute_profile_update_instance = InstituteProfileUpdate.from_json(json)
# print the JSON string representation of the object
print(InstituteProfileUpdate.to_json())

# convert the object into a dict
institute_profile_update_dict = institute_profile_update_instance.to_dict()
# create an instance of InstituteProfileUpdate from a dict
institute_profile_update_from_dict = InstituteProfileUpdate.from_dict(institute_profile_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


