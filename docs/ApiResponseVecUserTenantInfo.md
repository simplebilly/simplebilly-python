# ApiResponseVecUserTenantInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ApiResponseVecUserTenantInfoDataInner]**](ApiResponseVecUserTenantInfoDataInner.md) |  | [optional] 
**error** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.api_response_vec_user_tenant_info import ApiResponseVecUserTenantInfo

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseVecUserTenantInfo from a JSON string
api_response_vec_user_tenant_info_instance = ApiResponseVecUserTenantInfo.from_json(json)
# print the JSON string representation of the object
print(ApiResponseVecUserTenantInfo.to_json())

# convert the object into a dict
api_response_vec_user_tenant_info_dict = api_response_vec_user_tenant_info_instance.to_dict()
# create an instance of ApiResponseVecUserTenantInfo from a dict
api_response_vec_user_tenant_info_from_dict = ApiResponseVecUserTenantInfo.from_dict(api_response_vec_user_tenant_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


