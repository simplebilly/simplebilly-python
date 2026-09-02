# LegalDocument


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** | Plain text, &#x60;\\n\\n&#x60; separates paragraphs. | 
**doc_type** | [**LegalDocType**](LegalDocType.md) |  | 
**lang** | [**LanguageCode**](LanguageCode.md) |  | 
**title** | **str** |  | 

## Example

```python
from simplebilly_api.models.legal_document import LegalDocument

# TODO update the JSON string below
json = "{}"
# create an instance of LegalDocument from a JSON string
legal_document_instance = LegalDocument.from_json(json)
# print the JSON string representation of the object
print(LegalDocument.to_json())

# convert the object into a dict
legal_document_dict = legal_document_instance.to_dict()
# create an instance of LegalDocument from a dict
legal_document_from_dict = LegalDocument.from_dict(legal_document_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


