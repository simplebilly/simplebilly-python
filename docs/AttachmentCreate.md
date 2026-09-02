# AttachmentCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **str** | Contact this attachment belongs to (per-contact DMS). References the contact entity. | [optional] 
**file_name** | **str** |  | 
**file_size** | **int** |  | [optional] 
**mime_type** | **str** |  | [optional] 
**original_name** | **str** |  | 
**pdfa_path** | **str** |  | [optional] 
**sha256_hash** | **str** |  | [optional] 
**uploaded_by** | **UUID** |  | [optional] 

## Example

```python
from simplebilly_api.models.attachment_create import AttachmentCreate

# TODO update the JSON string below
json = "{}"
# create an instance of AttachmentCreate from a JSON string
attachment_create_instance = AttachmentCreate.from_json(json)
# print the JSON string representation of the object
print(AttachmentCreate.to_json())

# convert the object into a dict
attachment_create_dict = attachment_create_instance.to_dict()
# create an instance of AttachmentCreate from a dict
attachment_create_from_dict = AttachmentCreate.from_dict(attachment_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


