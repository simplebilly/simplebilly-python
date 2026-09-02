# DownPaymentInvoice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **str** |  | [optional] 
**contact_name** | **str** |  | [optional] 
**created_at** | **str** |  | [readonly] 
**currency** | **str** |  | 
**id** | **str** |  | 
**notes** | **str** |  | [optional] 
**paid_amount** | **str** |  | 
**total_amount** | **str** |  | 
**voucher_date** | **date** |  | 
**voucher_number** | **str** |  | [optional] 
**voucher_status** | **str** |  | 

## Example

```python
from simplebilly_api.models.down_payment_invoice import DownPaymentInvoice

# TODO update the JSON string below
json = "{}"
# create an instance of DownPaymentInvoice from a JSON string
down_payment_invoice_instance = DownPaymentInvoice.from_json(json)
# print the JSON string representation of the object
print(DownPaymentInvoice.to_json())

# convert the object into a dict
down_payment_invoice_dict = down_payment_invoice_instance.to_dict()
# create an instance of DownPaymentInvoice from a dict
down_payment_invoice_from_dict = DownPaymentInvoice.from_dict(down_payment_invoice_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


