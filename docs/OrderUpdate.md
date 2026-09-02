# OrderUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**audit_log** | **object** |  | [optional] 
**currency** | **str** |  | [optional] 
**customer_id** | **str** | References the customer entity. | [optional] 
**external_reference** | **str** |  | [optional] 
**invoice_address** | **object** |  | [optional] 
**items** | **object** |  | [optional] 
**language** | [**LanguageCode**](LanguageCode.md) |  | [optional] 
**order_status** | [**OrderStatus**](OrderStatus.md) |  | [optional] 
**payment_method** | [**PaymentMethod**](PaymentMethod.md) |  | [optional] 
**shipping_address** | **object** |  | [optional] 
**shipping_cost** | **str** |  | [optional] 
**shipping_method** | **str** |  | [optional] 
**shipping_weight** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] 
**total_cost** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.order_update import OrderUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of OrderUpdate from a JSON string
order_update_instance = OrderUpdate.from_json(json)
# print the JSON string representation of the object
print(OrderUpdate.to_json())

# convert the object into a dict
order_update_dict = order_update_instance.to_dict()
# create an instance of OrderUpdate from a dict
order_update_from_dict = OrderUpdate.from_dict(order_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


