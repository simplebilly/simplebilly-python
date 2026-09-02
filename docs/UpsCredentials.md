# UpsCredentials


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **str** | OAuth 2.0 client credentials from developer.ups.com. | 
**client_secret** | **str** |  | 
**shipper_number** | **str** | UPS account number; required for label creation, optional for rates/tracking. | [optional] 

## Example

```python
from simplebilly_api.models.ups_credentials import UpsCredentials

# TODO update the JSON string below
json = "{}"
# create an instance of UpsCredentials from a JSON string
ups_credentials_instance = UpsCredentials.from_json(json)
# print the JSON string representation of the object
print(UpsCredentials.to_json())

# convert the object into a dict
ups_credentials_dict = ups_credentials_instance.to_dict()
# create an instance of UpsCredentials from a dict
ups_credentials_from_dict = UpsCredentials.from_dict(ups_credentials_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


