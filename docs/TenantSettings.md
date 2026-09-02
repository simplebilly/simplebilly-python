# TenantSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**company_type** | [**CompanyType**](CompanyType.md) |  | 
**dpa_accepted_at** | **datetime** |  | [optional] 
**dpa_accepted_by** | **str** |  | [optional] 
**dpa_version** | **str** |  | [optional] 
**features** | **object** | Active feature toggles for the tenant. | 

## Example

```python
from simplebilly_api.models.tenant_settings import TenantSettings

# TODO update the JSON string below
json = "{}"
# create an instance of TenantSettings from a JSON string
tenant_settings_instance = TenantSettings.from_json(json)
# print the JSON string representation of the object
print(TenantSettings.to_json())

# convert the object into a dict
tenant_settings_dict = tenant_settings_instance.to_dict()
# create an instance of TenantSettings from a dict
tenant_settings_from_dict = TenantSettings.from_dict(tenant_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


