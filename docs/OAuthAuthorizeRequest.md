# OAuthAuthorizeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config** | **object** | Optional platform-specific config (e.g. Shopify &#x60;shop_domain&#x60;, &#x60;api_key&#x60;, &#x60;api_secret&#x60;) needed to build the authorization URL. | [optional] 
**platform** | **str** |  | 
**redirect_uri** | **str** |  | 

## Example

```python
from simplebilly_api.models.o_auth_authorize_request import OAuthAuthorizeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OAuthAuthorizeRequest from a JSON string
o_auth_authorize_request_instance = OAuthAuthorizeRequest.from_json(json)
# print the JSON string representation of the object
print(OAuthAuthorizeRequest.to_json())

# convert the object into a dict
o_auth_authorize_request_dict = o_auth_authorize_request_instance.to_dict()
# create an instance of OAuthAuthorizeRequest from a dict
o_auth_authorize_request_from_dict = OAuthAuthorizeRequest.from_dict(o_auth_authorize_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


