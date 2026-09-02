# DhlCredentials


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_key** | **str** | DHL-API-Key from developer.dhl.com (required for tracking). | 
**client_id** | **str** | Client credentials from the DHL developer app; required for label creation. | [optional] 
**client_secret** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.dhl_credentials import DhlCredentials

# TODO update the JSON string below
json = "{}"
# create an instance of DhlCredentials from a JSON string
dhl_credentials_instance = DhlCredentials.from_json(json)
# print the JSON string representation of the object
print(DhlCredentials.to_json())

# convert the object into a dict
dhl_credentials_dict = dhl_credentials_instance.to_dict()
# create an instance of DhlCredentials from a dict
dhl_credentials_from_dict = DhlCredentials.from_dict(dhl_credentials_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


