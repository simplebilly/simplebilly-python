# LegalDocumentReset

Optional filter for `POST /api/v1/legal/documents/reset`; empty body restores every document of the tenant.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**doc_type** | **str** |  | [optional] 
**lang** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.legal_document_reset import LegalDocumentReset

# TODO update the JSON string below
json = "{}"
# create an instance of LegalDocumentReset from a JSON string
legal_document_reset_instance = LegalDocumentReset.from_json(json)
# print the JSON string representation of the object
print(LegalDocumentReset.to_json())

# convert the object into a dict
legal_document_reset_dict = legal_document_reset_instance.to_dict()
# create an instance of LegalDocumentReset from a dict
legal_document_reset_from_dict = LegalDocumentReset.from_dict(legal_document_reset_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


