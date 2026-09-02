# OAuthCallbackRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**config** | **object** |  | [optional] 
**connection_id** | **str** |  | [optional] 
**platform** | **str** |  | 
**shop_domain** | **str** |  | [optional] 
**state** | **str** |  | 

## Example

```python
from simplebilly_api.models.o_auth_callback_request import OAuthCallbackRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OAuthCallbackRequest from a JSON string
o_auth_callback_request_instance = OAuthCallbackRequest.from_json(json)
# print the JSON string representation of the object
print(OAuthCallbackRequest.to_json())

# convert the object into a dict
o_auth_callback_request_dict = o_auth_callback_request_instance.to_dict()
# create an instance of OAuthCallbackRequest from a dict
o_auth_callback_request_from_dict = OAuthCallbackRequest.from_dict(o_auth_callback_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


