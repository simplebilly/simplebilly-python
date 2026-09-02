# Invoice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attachments** | **object** |  | [optional] 
**billing_period_end** | **date** |  | [optional] 
**billing_period_start** | **date** |  | [optional] 
**cancellation_date** | **date** |  | [optional] 
**cancellation_invoice_id** | **str** | References the invoice entity. | [optional] 
**cancellation_reason** | **str** |  | [optional] 
**contract_id** | **UUID** | References the contract entity. | [optional] 
**currency** | [**CurrencyCode**](CurrencyCode.md) |  | 
**customer_id** | **str** | References the customer entity. | [optional] 
**discount_amount** | **str** |  | [optional] 
**discount_days** | **int** |  | [optional] 
**discount_percentage** | **str** |  | [optional] 
**document_type** | [**DocumentType**](DocumentType.md) |  | [optional] 
**dunning_level** | **int** |  | [optional] 
**input_vat_amount** | **str** |  | [optional] 
**input_vat_deductible** | **bool** |  | [optional] 
**input_vat_percentage** | **str** |  | [optional] 
**introduction_text** | **str** |  | [optional] 
**invoice_type** | [**InvoiceType**](InvoiceType.md) |  | 
**is_cancelled** | **bool** |  | [optional] 
**is_draft** | **bool** |  | [optional] 
**is_eu_acquisition** | **bool** |  | [optional] 
**is_eu_delivery** | **bool** |  | [optional] 
**is_intra_community_acquisition** | **bool** |  | [optional] 
**is_reverse_charge** | **bool** |  | [optional] 
**issue_date** | **date** |  | 
**ledger_account** | **str** |  | [optional] 
**line_items** | **object** |  | 
**margin25a** | **bool** |  | [optional] 
**margin25a_gross** | **str** |  | [optional] 
**margin25a_purchase_price** | **str** |  | [optional] 
**notes** | **str** |  | [optional] 
**order_number** | **str** |  | [optional] 
**original_pdf_path** | **str** |  | [optional] 
**paid_amount** | **str** |  | [optional] 
**payment_due_date** | **date** |  | [optional] 
**payment_status** | [**PaymentStatus**](PaymentStatus.md) |  | [optional] 
**payment_terms_text** | **str** |  | [optional] 
**preceding_sales_voucher_id** | **str** | References the preceding sales voucher entity. | [optional] 
**preceding_sales_voucher_type** | [**PrecedingSalesVoucherType**](PrecedingSalesVoucherType.md) |  | [optional] 
**receipt_confirmation_available** | **bool** |  | [optional] 
**related_invoice_id** | **UUID** | References the invoice entity. | [optional] 
**relationship_type** | **str** |  | [optional] 
**sender_snapshot** | **object** |  | [optional] 
**sent_at** | **datetime** |  | [optional] 
**service_period_end** | **date** |  | [optional] 
**service_period_start** | **date** |  | [optional] 
**status** | [**InvoiceStatus**](InvoiceStatus.md) |  | 
**subtotal** | **str** |  | 
**supplier_id** | **str** | References the supplier entity. | [optional] 
**tax_exemption_reason** | **str** |  | [optional] 
**total_amount** | **str** |  | 
**total_tax** | **str** |  | 
**vat_country** | [**CountryCode**](CountryCode.md) |  | [optional] 
**vat_special_case** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.invoice import Invoice

# TODO update the JSON string below
json = "{}"
# create an instance of Invoice from a JSON string
invoice_instance = Invoice.from_json(json)
# print the JSON string representation of the object
print(Invoice.to_json())

# convert the object into a dict
invoice_dict = invoice_instance.to_dict()
# create an instance of Invoice from a dict
invoice_from_dict = Invoice.from_dict(invoice_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


