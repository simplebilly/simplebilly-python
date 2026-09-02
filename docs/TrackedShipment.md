# TrackedShipment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**carrier** | **str** |  | 
**events** | [**List[TrackingEvent]**](TrackingEvent.md) |  | 
**label_url** | **str** |  | [optional] 
**status** | **str** |  | 
**tracking_number** | **str** |  | [optional] 
**tracking_url** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.tracked_shipment import TrackedShipment

# TODO update the JSON string below
json = "{}"
# create an instance of TrackedShipment from a JSON string
tracked_shipment_instance = TrackedShipment.from_json(json)
# print the JSON string representation of the object
print(TrackedShipment.to_json())

# convert the object into a dict
tracked_shipment_dict = tracked_shipment_instance.to_dict()
# create an instance of TrackedShipment from a dict
tracked_shipment_from_dict = TrackedShipment.from_dict(tracked_shipment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


