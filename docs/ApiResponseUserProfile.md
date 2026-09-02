# ApiResponseUserProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ApiResponseUserProfileData**](ApiResponseUserProfileData.md) |  | [optional] 
**error** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.api_response_user_profile import ApiResponseUserProfile

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseUserProfile from a JSON string
api_response_user_profile_instance = ApiResponseUserProfile.from_json(json)
# print the JSON string representation of the object
print(ApiResponseUserProfile.to_json())

# convert the object into a dict
api_response_user_profile_dict = api_response_user_profile_instance.to_dict()
# create an instance of ApiResponseUserProfile from a dict
api_response_user_profile_from_dict = ApiResponseUserProfile.from_dict(api_response_user_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


