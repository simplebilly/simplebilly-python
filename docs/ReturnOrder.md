# ReturnOrder


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_contact_id** | **str** | References the contact entity. | [optional] 
**customer_name** | **str** |  | [optional] 
**line_items** | **object** | JSON array of &#x60;{product_id, name, quantity, condition, restock, batch_number?}&#x60;. | [optional] 
**notes** | **str** |  | [optional] 
**order_id** | **str** | References the order entity. | [optional] 
**order_number** | **str** |  | [optional] 
**return_number** | **str** |  | 
**return_reason** | **str** |  | [optional] 
**status** | [**ReturnOrderStatus**](ReturnOrderStatus.md) | One of: requested | received | inspected | restocked | closed | 
**warehouse_id** | **str** | Warehouse into which restockable items are returned. References the warehouse entity. | [optional] 

## Example

```python
from simplebilly_api.models.return_order import ReturnOrder

# TODO update the JSON string below
json = "{}"
# create an instance of ReturnOrder from a JSON string
return_order_instance = ReturnOrder.from_json(json)
# print the JSON string representation of the object
print(ReturnOrder.to_json())

# convert the object into a dict
return_order_dict = return_order_instance.to_dict()
# create an instance of ReturnOrder from a dict
return_order_from_dict = ReturnOrder.from_dict(return_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


