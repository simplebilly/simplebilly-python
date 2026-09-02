# ProformaInvoice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**converted_at** | **datetime** |  | [optional] 
**converted_to_invoice_id** | **str** | Set when the proforma was converted into a real invoice. References the invoice entity. | [optional] 
**currency** | [**CurrencyCode**](CurrencyCode.md) |  | 
**customer_id** | **str** | References the customer entity. | [optional] 
**customer_snapshot** | **object** | Snapshot of the recipient at issue time (address, VAT id, …). | [optional] 
**issue_date** | **date** |  | 
**line_items** | **object** |  | 
**notes** | **str** |  | [optional] 
**order_number** | **str** | Reference to the order/quote this proforma belongs to. | [optional] 
**payment_due_date** | **date** | Optional deadline the real invoice should carry after conversion. | [optional] 
**quotation_id** | **str** | References the quotation entity. | [optional] 
**status** | [**ProformaInvoiceStatus**](ProformaInvoiceStatus.md) | &#x60;draft&#x60; | &#x60;sent&#x60; | &#x60;converted&#x60;. | 
**subtotal** | **str** |  | 
**total_amount** | **str** |  | 
**total_tax** | **str** |  | 

## Example

```python
from simplebilly_api.models.proforma_invoice import ProformaInvoice

# TODO update the JSON string below
json = "{}"
# create an instance of ProformaInvoice from a JSON string
proforma_invoice_instance = ProformaInvoice.from_json(json)
# print the JSON string representation of the object
print(ProformaInvoice.to_json())

# convert the object into a dict
proforma_invoice_dict = proforma_invoice_instance.to_dict()
# create an instance of ProformaInvoice from a dict
proforma_invoice_from_dict = ProformaInvoice.from_dict(proforma_invoice_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


