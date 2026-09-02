# LegalDocumentUpsert

One document to upsert (`PUT /api/v1/legal/documents` body element).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | 
**doc_type** | **str** |  | 
**lang** | **str** |  | 
**title** | **str** |  | 

## Example

```python
from simplebilly_api.models.legal_document_upsert import LegalDocumentUpsert

# TODO update the JSON string below
json = "{}"
# create an instance of LegalDocumentUpsert from a JSON string
legal_document_upsert_instance = LegalDocumentUpsert.from_json(json)
# print the JSON string representation of the object
print(LegalDocumentUpsert.to_json())

# convert the object into a dict
legal_document_upsert_dict = legal_document_upsert_instance.to_dict()
# create an instance of LegalDocumentUpsert from a dict
legal_document_upsert_from_dict = LegalDocumentUpsert.from_dict(legal_document_upsert_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


