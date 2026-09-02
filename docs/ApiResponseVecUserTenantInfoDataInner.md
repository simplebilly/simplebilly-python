# ApiResponseVecUserTenantInfoDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**custom_domain** | **str** |  | [optional] 
**role** | **str** |  | 
**subdomain** | **str** |  | [optional] 
**tenant_id** | **UUID** |  | 
**tenant_name** | **str** |  | 

## Example

```python
from simplebilly_api.models.api_response_vec_user_tenant_info_data_inner import ApiResponseVecUserTenantInfoDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseVecUserTenantInfoDataInner from a JSON string
api_response_vec_user_tenant_info_data_inner_instance = ApiResponseVecUserTenantInfoDataInner.from_json(json)
# print the JSON string representation of the object
print(ApiResponseVecUserTenantInfoDataInner.to_json())

# convert the object into a dict
api_response_vec_user_tenant_info_data_inner_dict = api_response_vec_user_tenant_info_data_inner_instance.to_dict()
# create an instance of ApiResponseVecUserTenantInfoDataInner from a dict
api_response_vec_user_tenant_info_data_inner_from_dict = ApiResponseVecUserTenantInfoDataInner.from_dict(api_response_vec_user_tenant_info_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


