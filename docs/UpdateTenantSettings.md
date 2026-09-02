# UpdateTenantSettings

Request payload for updating tenant settings.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**company_type** | [**CompanyType**](CompanyType.md) |  | 
**features** | [**PartialFeatureSettings**](PartialFeatureSettings.md) |  | [optional] 

## Example

```python
from simplebilly_api.models.update_tenant_settings import UpdateTenantSettings

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateTenantSettings from a JSON string
update_tenant_settings_instance = UpdateTenantSettings.from_json(json)
# print the JSON string representation of the object
print(UpdateTenantSettings.to_json())

# convert the object into a dict
update_tenant_settings_dict = update_tenant_settings_instance.to_dict()
# create an instance of UpdateTenantSettings from a dict
update_tenant_settings_from_dict = UpdateTenantSettings.from_dict(update_tenant_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


