# PackingCompleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**notes** | **str** |  | [optional] 
**order_number** | **str** |  | 
**shipment_id** | **str** |  | [optional] 
**video_url** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.packing_complete_request import PackingCompleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PackingCompleteRequest from a JSON string
packing_complete_request_instance = PackingCompleteRequest.from_json(json)
# print the JSON string representation of the object
print(PackingCompleteRequest.to_json())

# convert the object into a dict
packing_complete_request_dict = packing_complete_request_instance.to_dict()
# create an instance of PackingCompleteRequest from a dict
packing_complete_request_from_dict = PackingCompleteRequest.from_dict(packing_complete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


