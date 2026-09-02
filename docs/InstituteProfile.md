# InstituteProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**institute_type** | [**InstituteType**](InstituteType.md) | Institutsart: \&quot;kein\&quot; | \&quot;kreditinstitut\&quot; | \&quot;finanzdienstleistungsinstitut\&quot; | \&quot;finanzunternehmen\&quot; | \&quot;versicherung\&quot;. | [optional] 
**kapitalmarktorientiert** | **bool** | Kapitalmarktorientierung (§ 325 Abs. 4 HGB): Offenlegungsfrist 4 statt 12 Monate. | [optional] 

## Example

```python
from simplebilly_api.models.institute_profile import InstituteProfile

# TODO update the JSON string below
json = "{}"
# create an instance of InstituteProfile from a JSON string
institute_profile_instance = InstituteProfile.from_json(json)
# print the JSON string representation of the object
print(InstituteProfile.to_json())

# convert the object into a dict
institute_profile_dict = institute_profile_instance.to_dict()
# create an instance of InstituteProfile from a dict
institute_profile_from_dict = InstituteProfile.from_dict(institute_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


