# ShipmentStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delivered_at** | **str** |  | [optional] 
**signed_by** | **str** |  | [optional] 
**status** | **str** |  | 
**tracking_number** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.shipment_status_update import ShipmentStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ShipmentStatusUpdate from a JSON string
shipment_status_update_instance = ShipmentStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(ShipmentStatusUpdate.to_json())

# convert the object into a dict
shipment_status_update_dict = shipment_status_update_instance.to_dict()
# create an instance of ShipmentStatusUpdate from a dict
shipment_status_update_from_dict = ShipmentStatusUpdate.from_dict(shipment_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


