# UserTenantInfo


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
from simplebilly_api.models.user_tenant_info import UserTenantInfo

# TODO update the JSON string below
json = "{}"
# create an instance of UserTenantInfo from a JSON string
user_tenant_info_instance = UserTenantInfo.from_json(json)
# print the JSON string representation of the object
print(UserTenantInfo.to_json())

# convert the object into a dict
user_tenant_info_dict = user_tenant_info_instance.to_dict()
# create an instance of UserTenantInfo from a dict
user_tenant_info_from_dict = UserTenantInfo.from_dict(user_tenant_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


