# Shipment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delivered_at** | **datetime** |  | [optional] 
**label_url** | **str** |  | [optional] 
**line_items_shipment** | **object** |  | [optional] 
**order_id** | **str** | References the order entity. | 
**recipient_address** | **object** |  | [optional] 
**shipment_date** | **date** |  | 
**shipping_carrier** | **str** |  | 
**shipping_cost** | **str** |  | [optional] 
**shipping_method** | **str** |  | [optional] 
**signed_by** | **str** |  | [optional] 
**status** | **str** |  | 
**tracking_events** | **object** | Latest carrier tracking events (from the live tracking API). | [optional] 
**tracking_number** | **str** |  | [optional] 
**tracking_url** | **str** |  | [optional] 
**weight_kg** | **float** |  | [optional] 

## Example

```python
from simplebilly_api.models.shipment import Shipment

# TODO update the JSON string below
json = "{}"
# create an instance of Shipment from a JSON string
shipment_instance = Shipment.from_json(json)
# print the JSON string representation of the object
print(Shipment.to_json())

# convert the object into a dict
shipment_dict = shipment_instance.to_dict()
# create an instance of Shipment from a dict
shipment_from_dict = Shipment.from_dict(shipment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


