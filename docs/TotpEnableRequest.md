# TotpEnableRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 

## Example

```python
from simplebilly_api.models.totp_enable_request import TotpEnableRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TotpEnableRequest from a JSON string
totp_enable_request_instance = TotpEnableRequest.from_json(json)
# print the JSON string representation of the object
print(TotpEnableRequest.to_json())

# convert the object into a dict
totp_enable_request_dict = totp_enable_request_instance.to_dict()
# create an instance of TotpEnableRequest from a dict
totp_enable_request_from_dict = TotpEnableRequest.from_dict(totp_enable_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


