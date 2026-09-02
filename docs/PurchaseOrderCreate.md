# PurchaseOrderCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **str** |  | [optional] 
**delivery_address** | **object** |  | [optional] 
**expected_delivery_date** | **date** |  | [optional] 
**line_items** | **object** | JSON array of &#x60;{product_id, name, quantity, unit_price_net, tax_rate, delivery_date}&#x60;. | [optional] 
**notes** | **str** |  | [optional] 
**order_date** | **date** |  | 
**po_number** | **str** |  | 
**status** | [**PurchaseOrderStatus**](PurchaseOrderStatus.md) | One of: draft | ordered | partially_received | received | cancelled | 
**supplier_contact_id** | **str** | References the supplier entity. | [optional] 
**supplier_name** | **str** |  | [optional] 
**total_gross_amount** | **str** |  | [optional] 
**total_net_amount** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.purchase_order_create import PurchaseOrderCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseOrderCreate from a JSON string
purchase_order_create_instance = PurchaseOrderCreate.from_json(json)
# print the JSON string representation of the object
print(PurchaseOrderCreate.to_json())

# convert the object into a dict
purchase_order_create_dict = purchase_order_create_instance.to_dict()
# create an instance of PurchaseOrderCreate from a dict
purchase_order_create_from_dict = PurchaseOrderCreate.from_dict(purchase_order_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


