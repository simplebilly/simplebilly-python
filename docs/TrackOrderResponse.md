# TrackOrderResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order_number** | **str** |  | 
**order_status** | **str** |  | 
**shipments** | [**List[TrackedShipment]**](TrackedShipment.md) |  | 

## Example

```python
from simplebilly_api.models.track_order_response import TrackOrderResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TrackOrderResponse from a JSON string
track_order_response_instance = TrackOrderResponse.from_json(json)
# print the JSON string representation of the object
print(TrackOrderResponse.to_json())

# convert the object into a dict
track_order_response_dict = track_order_response_instance.to_dict()
# create an instance of TrackOrderResponse from a dict
track_order_response_from_dict = TrackOrderResponse.from_dict(track_order_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


