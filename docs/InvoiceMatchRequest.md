# InvoiceMatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**supplier_invoice_id** | **str** |  | 

## Example

```python
from simplebilly_api.models.invoice_match_request import InvoiceMatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceMatchRequest from a JSON string
invoice_match_request_instance = InvoiceMatchRequest.from_json(json)
# print the JSON string representation of the object
print(InvoiceMatchRequest.to_json())

# convert the object into a dict
invoice_match_request_dict = invoice_match_request_instance.to_dict()
# create an instance of InvoiceMatchRequest from a dict
invoice_match_request_from_dict = InvoiceMatchRequest.from_dict(invoice_match_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


