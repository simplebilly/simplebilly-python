# GdprTenant


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**role** | **str** |  | 
**tenant_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.gdpr_tenant import GdprTenant

# TODO update the JSON string below
json = "{}"
# create an instance of GdprTenant from a JSON string
gdpr_tenant_instance = GdprTenant.from_json(json)
# print the JSON string representation of the object
print(GdprTenant.to_json())

# convert the object into a dict
gdpr_tenant_dict = gdpr_tenant_instance.to_dict()
# create an instance of GdprTenant from a dict
gdpr_tenant_from_dict = GdprTenant.from_dict(gdpr_tenant_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


