# Attachment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **str** | Contact this attachment belongs to (per-contact DMS). References the contact entity. | [optional] 
**file_name** | **str** |  | 
**file_size** | **int** |  | [optional] 
**mime_type** | **str** |  | [optional] 
**ocr_text** | **str** | Raw text extracted by client-side OCR (tesseract.js), if run. | [optional] 
**original_name** | **str** |  | 
**pdfa_path** | **str** |  | [optional] 
**sha256_hash** | **str** |  | [optional] 
**uploaded_by** | **UUID** |  | [optional] 

## Example

```python
from simplebilly_api.models.attachment import Attachment

# TODO update the JSON string below
json = "{}"
# create an instance of Attachment from a JSON string
attachment_instance = Attachment.from_json(json)
# print the JSON string representation of the object
print(Attachment.to_json())

# convert the object into a dict
attachment_dict = attachment_instance.to_dict()
# create an instance of Attachment from a dict
attachment_from_dict = Attachment.from_dict(attachment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


