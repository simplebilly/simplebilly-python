# GatewayOAuthAuthorizeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gateway_type** | **str** |  | 
**redirect_uri** | **str** |  | 

## Example

```python
from simplebilly_api.models.gateway_o_auth_authorize_request import GatewayOAuthAuthorizeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GatewayOAuthAuthorizeRequest from a JSON string
gateway_o_auth_authorize_request_instance = GatewayOAuthAuthorizeRequest.from_json(json)
# print the JSON string representation of the object
print(GatewayOAuthAuthorizeRequest.to_json())

# convert the object into a dict
gateway_o_auth_authorize_request_dict = gateway_o_auth_authorize_request_instance.to_dict()
# create an instance of GatewayOAuthAuthorizeRequest from a dict
gateway_o_auth_authorize_request_from_dict = GatewayOAuthAuthorizeRequest.from_dict(gateway_o_auth_authorize_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


