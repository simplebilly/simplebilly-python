# QuotationCreate


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
**tax_condition** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**voucher_date** | **date** |  | 
**voucher_status** | [**VoucherStatus**](VoucherStatus.md) |  | 

## Example

```python
from simplebilly_api.models.quotation_create import QuotationCreate

# TODO update the JSON string below
json = "{}"
# create an instance of QuotationCreate from a JSON string
quotation_create_instance = QuotationCreate.from_json(json)
# print the JSON string representation of the object
print(QuotationCreate.to_json())

# convert the object into a dict
quotation_create_dict = quotation_create_instance.to_dict()
# create an instance of QuotationCreate from a dict
quotation_create_from_dict = QuotationCreate.from_dict(quotation_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


