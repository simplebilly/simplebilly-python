# OrderConfirmationCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **object** |  | [optional] 
**confirmation_number** | **str** |  | [optional] 
**contact_id** | **str** | References the contact entity. | [optional] 
**contact_name** | **str** |  | [optional] 
**currency** | **str** |  | 
**files** | **object** |  | [optional] 
**introduction** | **str** |  | [optional] 
**line_items** | **object** |  | [optional] 
**preceding_sales_voucher_id** | **str** | References the preceding sales voucher entity. | [optional] 
**preceding_sales_voucher_type** | [**PrecedingSalesVoucherType**](PrecedingSalesVoucherType.md) |  | [optional] 
**remark** | **str** |  | [optional] 
**tax_condition** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**voucher_date** | **date** |  | 
**voucher_status** | [**VoucherStatus**](VoucherStatus.md) |  | 

## Example

```python
from simplebilly_api.models.order_confirmation_create import OrderConfirmationCreate

# TODO update the JSON string below
json = "{}"
# create an instance of OrderConfirmationCreate from a JSON string
order_confirmation_create_instance = OrderConfirmationCreate.from_json(json)
# print the JSON string representation of the object
print(OrderConfirmationCreate.to_json())

# convert the object into a dict
order_confirmation_create_dict = order_confirmation_create_instance.to_dict()
# create an instance of OrderConfirmationCreate from a dict
order_confirmation_create_from_dict = OrderConfirmationCreate.from_dict(order_confirmation_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


