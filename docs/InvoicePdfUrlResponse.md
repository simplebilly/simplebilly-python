# InvoicePdfUrlResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | 

## Example

```python
from simplebilly_api.models.invoice_pdf_url_response import InvoicePdfUrlResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InvoicePdfUrlResponse from a JSON string
invoice_pdf_url_response_instance = InvoicePdfUrlResponse.from_json(json)
# print the JSON string representation of the object
print(InvoicePdfUrlResponse.to_json())

# convert the object into a dict
invoice_pdf_url_response_dict = invoice_pdf_url_response_instance.to_dict()
# create an instance of InvoicePdfUrlResponse from a dict
invoice_pdf_url_response_from_dict = InvoicePdfUrlResponse.from_dict(invoice_pdf_url_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


