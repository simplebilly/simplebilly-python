# Voucher


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category_id** | **str** |  | [optional] 
**contact_id** | **str** | References the contact entity. | [optional] 
**contact_name** | **str** |  | [optional] 
**currency** | **str** |  | 
**description** | **str** |  | [optional] 
**file_attachments** | **object** |  | [optional] 
**line_items** | **object** |  | [optional] 
**metadata** | **object** |  | [optional] 
**notes** | **str** |  | [optional] 
**open_amount** | **str** |  | [optional] 
**paid_date** | **date** |  | [optional] 
**payment_status** | [**PaymentStatus**](PaymentStatus.md) |  | [optional] 
**tax_amounts** | **object** |  | [optional] 
**tax_condition** | **str** |  | [optional] 
**total_gross_amount** | **str** |  | [optional] 
**total_net_amount** | **str** |  | [optional] 
**voucher_date** | **date** |  | 
**voucher_number** | **str** |  | [optional] 
**voucher_status** | [**VoucherStatus**](VoucherStatus.md) |  | 
**voucher_type** | [**VoucherType**](VoucherType.md) |  | 

## Example

```python
from simplebilly_api.models.voucher import Voucher

# TODO update the JSON string below
json = "{}"
# create an instance of Voucher from a JSON string
voucher_instance = Voucher.from_json(json)
# print the JSON string representation of the object
print(Voucher.to_json())

# convert the object into a dict
voucher_dict = voucher_instance.to_dict()
# create an instance of Voucher from a dict
voucher_from_dict = Voucher.from_dict(voucher_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


