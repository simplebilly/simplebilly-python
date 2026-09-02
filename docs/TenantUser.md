# TenantUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**email_verified** | **bool** |  | 
**is_active** | **bool** |  | 
**joined_at** | **datetime** |  | 
**last_login** | **datetime** |  | [optional] 
**name** | **str** |  | 
**permissions** | **List[str]** |  | 
**role** | **str** |  | 
**user_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.tenant_user import TenantUser

# TODO update the JSON string below
json = "{}"
# create an instance of TenantUser from a JSON string
tenant_user_instance = TenantUser.from_json(json)
# print the JSON string representation of the object
print(TenantUser.to_json())

# convert the object into a dict
tenant_user_dict = tenant_user_instance.to_dict()
# create an instance of TenantUser from a dict
tenant_user_from_dict = TenantUser.from_dict(tenant_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


