# ShippingCredentials

Per-tenant credentials for real shipping provider APIs (stored in the `shipping` key of the settings JSON blob). Auth is either OAuth client credentials (UPS) or a user-supplied API key (DHL).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dhl** | [**DhlCredentials**](DhlCredentials.md) |  | [optional] 
**ups** | [**UpsCredentials**](UpsCredentials.md) |  | [optional] 

## Example

```python
from simplebilly_api.models.shipping_credentials import ShippingCredentials

# TODO update the JSON string below
json = "{}"
# create an instance of ShippingCredentials from a JSON string
shipping_credentials_instance = ShippingCredentials.from_json(json)
# print the JSON string representation of the object
print(ShippingCredentials.to_json())

# convert the object into a dict
shipping_credentials_dict = shipping_credentials_instance.to_dict()
# create an instance of ShippingCredentials from a dict
shipping_credentials_from_dict = ShippingCredentials.from_dict(shipping_credentials_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


