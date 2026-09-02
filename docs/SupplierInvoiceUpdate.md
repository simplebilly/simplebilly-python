# SupplierInvoiceUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **str** |  | [optional] 
**goods_receipt_id** | **str** | References the goods receipt entity. | [optional] 
**invoice_date** | **date** |  | [optional] 
**invoice_number** | **str** |  | [optional] 
**line_items** | **object** | JSON array of &#x60;{product_id, name, quantity, unitPriceNet, taxRate}&#x60;. | [optional] 
**notes** | **str** |  | [optional] 
**purchase_order_id** | **str** | References the purchase order entity. | [optional] 
**status** | [**SupplierInvoiceStatus**](SupplierInvoiceStatus.md) | One of: draft | matched | has_variances | posted | cancelled | [optional] 
**supplier_contact_id** | **str** | References the supplier entity. | [optional] 
**supplier_name** | **str** |  | [optional] 
**total_gross_amount** | **str** |  | [optional] 
**total_net_amount** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.supplier_invoice_update import SupplierInvoiceUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of SupplierInvoiceUpdate from a JSON string
supplier_invoice_update_instance = SupplierInvoiceUpdate.from_json(json)
# print the JSON string representation of the object
print(SupplierInvoiceUpdate.to_json())

# convert the object into a dict
supplier_invoice_update_dict = supplier_invoice_update_instance.to_dict()
# create an instance of SupplierInvoiceUpdate from a dict
supplier_invoice_update_from_dict = SupplierInvoiceUpdate.from_dict(supplier_invoice_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


