# OrderCreate


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
from simplebilly_api.models.order_create import OrderCreate

# TODO update the JSON string below
json = "{}"
# create an instance of OrderCreate from a JSON string
order_create_instance = OrderCreate.from_json(json)
# print the JSON string representation of the object
print(OrderCreate.to_json())

# convert the object into a dict
order_create_dict = order_create_instance.to_dict()
# create an instance of OrderCreate from a dict
order_create_from_dict = OrderCreate.from_dict(order_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


