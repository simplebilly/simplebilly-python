# DeliveryNoteCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **object** |  | [optional] 
**contact_id** | **str** | References the contact entity. | [optional] 
**contact_name** | **str** |  | [optional] 
**currency** | **str** |  | 
**delivery_date** | **date** |  | [optional] 
**delivery_note_number** | **str** |  | [optional] 
**files** | **object** |  | [optional] 
**introduction** | **str** |  | [optional] 
**line_items** | **object** |  | [optional] 
**preceding_sales_voucher_id** | **str** | References the preceding sales voucher entity. | [optional] 
**preceding_sales_voucher_type** | [**PrecedingSalesVoucherType**](PrecedingSalesVoucherType.md) |  | [optional] 
**remark** | **str** |  | [optional] 
**shipping_date** | **date** |  | [optional] 
**shipping_method** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**voucher_date** | **date** |  | 
**voucher_status** | [**VoucherStatus**](VoucherStatus.md) |  | 

## Example

```python
from simplebilly_api.models.delivery_note_create import DeliveryNoteCreate

# TODO update the JSON string below
json = "{}"
# create an instance of DeliveryNoteCreate from a JSON string
delivery_note_create_instance = DeliveryNoteCreate.from_json(json)
# print the JSON string representation of the object
print(DeliveryNoteCreate.to_json())

# convert the object into a dict
delivery_note_create_dict = delivery_note_create_instance.to_dict()
# create an instance of DeliveryNoteCreate from a dict
delivery_note_create_from_dict = DeliveryNoteCreate.from_dict(delivery_note_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


