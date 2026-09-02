# GatewayOAuthCallbackRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**gateway_type** | **str** |  | 
**redirect_uri** | **str** |  | 
**state** | **str** |  | 

## Example

```python
from simplebilly_api.models.gateway_o_auth_callback_request import GatewayOAuthCallbackRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GatewayOAuthCallbackRequest from a JSON string
gateway_o_auth_callback_request_instance = GatewayOAuthCallbackRequest.from_json(json)
# print the JSON string representation of the object
print(GatewayOAuthCallbackRequest.to_json())

# convert the object into a dict
gateway_o_auth_callback_request_dict = gateway_o_auth_callback_request_instance.to_dict()
# create an instance of GatewayOAuthCallbackRequest from a dict
gateway_o_auth_callback_request_from_dict = GatewayOAuthCallbackRequest.from_dict(gateway_o_auth_callback_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


