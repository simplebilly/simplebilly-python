# InvoiceLineItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**article_number** | **str** |  | [optional] 
**description** | **str** |  | 
**discount_amount** | **str** |  | [optional] 
**discount_percentage** | **str** |  | [optional] 
**input_vat_deductible** | **bool** |  | [optional] 
**input_vat_rate** | **str** |  | [optional] 
**is_intra_community_acquisition** | **bool** |  | [optional] 
**is_margin_25a** | **bool** |  | [optional] 
**ledger_account** | **str** |  | [optional] 
**line_total** | **str** |  | 
**line_total_gross** | **str** |  | [optional] 
**margin_25a_purchase_price** | **str** |  | [optional] 
**meter_point_id** | **UUID** |  | [optional] 
**position** | **int** |  | 
**price_components** | **object** |  | [optional] 
**product_id** | **UUID** |  | [optional] 
**product_sku** | **str** |  | [optional] 
**quantity** | **str** |  | 
**supplier_article_number** | **str** |  | [optional] 
**tax_rate** | **str** |  | [optional] 
**unit** | **object** |  | 
**unit_price** | **str** |  | 
**usage_data_id** | **UUID** |  | [optional] 
**vat_rate_nominal** | **str** |  | [optional] 
**vat_special_case** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.invoice_line_item import InvoiceLineItem

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceLineItem from a JSON string
invoice_line_item_instance = InvoiceLineItem.from_json(json)
# print the JSON string representation of the object
print(InvoiceLineItem.to_json())

# convert the object into a dict
invoice_line_item_dict = invoice_line_item_instance.to_dict()
# create an instance of InvoiceLineItem from a dict
invoice_line_item_from_dict = InvoiceLineItem.from_dict(invoice_line_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


