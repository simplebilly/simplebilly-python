# ProformaInvoiceUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**converted_at** | **datetime** |  | [optional] 
**converted_to_invoice_id** | **str** | Set when the proforma was converted into a real invoice. References the invoice entity. | [optional] 
**currency** | [**CurrencyCode**](CurrencyCode.md) |  | [optional] 
**customer_id** | **str** | References the customer entity. | [optional] 
**customer_snapshot** | **object** | Snapshot of the recipient at issue time (address, VAT id, …). | [optional] 
**issue_date** | **date** |  | [optional] 
**line_items** | **object** |  | [optional] 
**notes** | **str** |  | [optional] 
**order_number** | **str** | Reference to the order/quote this proforma belongs to. | [optional] 
**payment_due_date** | **date** | Optional deadline the real invoice should carry after conversion. | [optional] 
**quotation_id** | **str** | References the quotation entity. | [optional] 
**status** | [**ProformaInvoiceStatus**](ProformaInvoiceStatus.md) | &#x60;draft&#x60; | &#x60;sent&#x60; | &#x60;converted&#x60;. | [optional] 
**subtotal** | **str** |  | [optional] 
**total_amount** | **str** |  | [optional] 
**total_tax** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.proforma_invoice_update import ProformaInvoiceUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ProformaInvoiceUpdate from a JSON string
proforma_invoice_update_instance = ProformaInvoiceUpdate.from_json(json)
# print the JSON string representation of the object
print(ProformaInvoiceUpdate.to_json())

# convert the object into a dict
proforma_invoice_update_dict = proforma_invoice_update_instance.to_dict()
# create an instance of ProformaInvoiceUpdate from a dict
proforma_invoice_update_from_dict = ProformaInvoiceUpdate.from_dict(proforma_invoice_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


