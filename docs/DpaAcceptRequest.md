# DpaAcceptRequest

Request body to record DPA acceptance (`PUT /api/v1/gdpr/dpa`).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accepted_by_name** | **str** |  | 
**version** | **str** |  | 

## Example

```python
from simplebilly_api.models.dpa_accept_request import DpaAcceptRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DpaAcceptRequest from a JSON string
dpa_accept_request_instance = DpaAcceptRequest.from_json(json)
# print the JSON string representation of the object
print(DpaAcceptRequest.to_json())

# convert the object into a dict
dpa_accept_request_dict = dpa_accept_request_instance.to_dict()
# create an instance of DpaAcceptRequest from a dict
dpa_accept_request_from_dict = DpaAcceptRequest.from_dict(dpa_accept_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


