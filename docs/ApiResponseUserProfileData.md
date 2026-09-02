# ApiResponseUserProfileData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | 
**email** | **str** |  | 
**email_verified** | **bool** |  | 
**first_name** | **str** |  | 
**full_name** | **str** |  | 
**id** | **UUID** |  | 
**last_name** | **str** |  | 

## Example

```python
from simplebilly_api.models.api_response_user_profile_data import ApiResponseUserProfileData

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseUserProfileData from a JSON string
api_response_user_profile_data_instance = ApiResponseUserProfileData.from_json(json)
# print the JSON string representation of the object
print(ApiResponseUserProfileData.to_json())

# convert the object into a dict
api_response_user_profile_data_dict = api_response_user_profile_data_instance.to_dict()
# create an instance of ApiResponseUserProfileData from a dict
api_response_user_profile_data_from_dict = ApiResponseUserProfileData.from_dict(api_response_user_profile_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


