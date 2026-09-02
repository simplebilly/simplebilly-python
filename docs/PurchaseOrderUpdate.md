# PurchaseOrderUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **str** |  | [optional] 
**delivery_address** | **object** |  | [optional] 
**expected_delivery_date** | **date** |  | [optional] 
**line_items** | **object** | JSON array of &#x60;{product_id, name, quantity, unit_price_net, tax_rate, delivery_date}&#x60;. | [optional] 
**notes** | **str** |  | [optional] 
**order_date** | **date** |  | [optional] 
**po_number** | **str** |  | [optional] 
**status** | [**PurchaseOrderStatus**](PurchaseOrderStatus.md) | One of: draft | ordered | partially_received | received | cancelled | [optional] 
**supplier_contact_id** | **str** | References the supplier entity. | [optional] 
**supplier_name** | **str** |  | [optional] 
**total_gross_amount** | **str** |  | [optional] 
**total_net_amount** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.purchase_order_update import PurchaseOrderUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseOrderUpdate from a JSON string
purchase_order_update_instance = PurchaseOrderUpdate.from_json(json)
# print the JSON string representation of the object
print(PurchaseOrderUpdate.to_json())

# convert the object into a dict
purchase_order_update_dict = purchase_order_update_instance.to_dict()
# create an instance of PurchaseOrderUpdate from a dict
purchase_order_update_from_dict = PurchaseOrderUpdate.from_dict(purchase_order_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


