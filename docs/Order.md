# Order


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**audit_log** | **object** |  | [optional] 
**currency** | **str** |  | 
**customer_id** | **str** | References the customer entity. | 
**external_reference** | **str** |  | [optional] 
**invoice_address** | **object** |  | [optional] 
**items** | **object** |  | [optional] 
**language** | [**LanguageCode**](LanguageCode.md) |  | [optional] 
**order_status** | [**OrderStatus**](OrderStatus.md) |  | 
**payment_method** | [**PaymentMethod**](PaymentMethod.md) |  | 
**shipping_address** | **object** |  | [optional] 
**shipping_cost** | **str** |  | 
**shipping_method** | **str** |  | 
**shipping_weight** | **str** |  | 
**tags** | **List[str]** |  | 
**total_cost** | **str** |  | 

## Example

```python
from simplebilly_api.models.order import Order

# TODO update the JSON string below
json = "{}"
# create an instance of Order from a JSON string
order_instance = Order.from_json(json)
# print the JSON string representation of the object
print(Order.to_json())

# convert the object into a dict
order_dict = order_instance.to_dict()
# create an instance of Order from a dict
order_from_dict = Order.from_dict(order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


