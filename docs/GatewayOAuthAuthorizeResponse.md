# GatewayOAuthAuthorizeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**authorization_url** | **str** |  | 
**state** | **str** |  | 

## Example

```python
from simplebilly_api.models.gateway_o_auth_authorize_response import GatewayOAuthAuthorizeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GatewayOAuthAuthorizeResponse from a JSON string
gateway_o_auth_authorize_response_instance = GatewayOAuthAuthorizeResponse.from_json(json)
# print the JSON string representation of the object
print(GatewayOAuthAuthorizeResponse.to_json())

# convert the object into a dict
gateway_o_auth_authorize_response_dict = gateway_o_auth_authorize_response_instance.to_dict()
# create an instance of GatewayOAuthAuthorizeResponse from a dict
gateway_o_auth_authorize_response_from_dict = GatewayOAuthAuthorizeResponse.from_dict(gateway_o_auth_authorize_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


