# TrackOrderRequest

Refresh tracking for a shipment from the live carrier API and store the latest status + events on the shipment row.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**order_number** | **str** |  | 

## Example

```python
from simplebilly_api.models.track_order_request import TrackOrderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TrackOrderRequest from a JSON string
track_order_request_instance = TrackOrderRequest.from_json(json)
# print the JSON string representation of the object
print(TrackOrderRequest.to_json())

# convert the object into a dict
track_order_request_dict = track_order_request_instance.to_dict()
# create an instance of TrackOrderRequest from a dict
track_order_request_from_dict = TrackOrderRequest.from_dict(track_order_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


