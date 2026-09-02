# SupplierInvoiceStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.supplier_invoice_status_update import SupplierInvoiceStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of SupplierInvoiceStatusUpdate from a JSON string
supplier_invoice_status_update_instance = SupplierInvoiceStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(SupplierInvoiceStatusUpdate.to_json())

# convert the object into a dict
supplier_invoice_status_update_dict = supplier_invoice_status_update_instance.to_dict()
# create an instance of SupplierInvoiceStatusUpdate from a dict
supplier_invoice_status_update_from_dict = SupplierInvoiceStatusUpdate.from_dict(supplier_invoice_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


