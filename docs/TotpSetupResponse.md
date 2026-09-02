# TotpSetupResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**backup_codes** | **List[str]** |  | 
**qr_code_url** | **str** |  | 
**secret** | **str** |  | 

## Example

```python
from simplebilly_api.models.totp_setup_response import TotpSetupResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TotpSetupResponse from a JSON string
totp_setup_response_instance = TotpSetupResponse.from_json(json)
# print the JSON string representation of the object
print(TotpSetupResponse.to_json())

# convert the object into a dict
totp_setup_response_dict = totp_setup_response_instance.to_dict()
# create an instance of TotpSetupResponse from a dict
totp_setup_response_from_dict = TotpSetupResponse.from_dict(totp_setup_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


