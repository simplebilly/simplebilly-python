# Quotation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **object** |  | [optional] 
**contact_id** | **str** | References the contact entity. | [optional] 
**contact_name** | **str** |  | [optional] 
**currency** | **str** |  | 
**expiration_date** | **date** |  | [optional] 
**files** | **object** |  | [optional] 
**introduction** | **str** |  | [optional] 
**line_items** | **object** |  | [optional] 
**preceding_sales_voucher_id** | **str** | References the preceding sales voucher entity. | [optional] 
**preceding_sales_voucher_type** | [**PrecedingSalesVoucherType**](PrecedingSalesVoucherType.md) |  | [optional] 
**quotation_number** | **str** |  | [optional] 
**remark** | **str** |  | [optional] 
**subtotal** | **str** |  | [optional] 
**tax_condition** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**total_amount** | **str** |  | [optional] 
**total_tax** | **str** |  | [optional] 
**voucher_date** | **date** |  | 
**voucher_status** | [**VoucherStatus**](VoucherStatus.md) |  | 

## Example

```python
from simplebilly_api.models.quotation import Quotation

# TODO update the JSON string below
json = "{}"
# create an instance of Quotation from a JSON string
quotation_instance = Quotation.from_json(json)
# print the JSON string representation of the object
print(Quotation.to_json())

# convert the object into a dict
quotation_dict = quotation_instance.to_dict()
# create an instance of Quotation from a dict
quotation_from_dict = Quotation.from_dict(quotation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


