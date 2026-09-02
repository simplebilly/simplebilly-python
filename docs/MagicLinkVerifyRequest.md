# MagicLinkVerifyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**token** | **str** |  | 

## Example

```python
from simplebilly_api.models.magic_link_verify_request import MagicLinkVerifyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MagicLinkVerifyRequest from a JSON string
magic_link_verify_request_instance = MagicLinkVerifyRequest.from_json(json)
# print the JSON string representation of the object
print(MagicLinkVerifyRequest.to_json())

# convert the object into a dict
magic_link_verify_request_dict = magic_link_verify_request_instance.to_dict()
# create an instance of MagicLinkVerifyRequest from a dict
magic_link_verify_request_from_dict = MagicLinkVerifyRequest.from_dict(magic_link_verify_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


