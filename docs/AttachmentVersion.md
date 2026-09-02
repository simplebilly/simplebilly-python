# AttachmentVersion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attachment_id** | **UUID** | Parent attachment whose history this row records. | 
**file_name** | **str** | Storage key of this version&#39;s bytes. | 
**file_size** | **int** |  | [optional] 
**mime_type** | **str** |  | [optional] 
**original_name** | **str** |  | [optional] 
**sha256_hash** | **str** |  | [optional] 
**uploaded_by** | **UUID** |  | [optional] 
**version_number** | **int** | 1-based; ascending per attachment in upload order. | 

## Example

```python
from simplebilly_api.models.attachment_version import AttachmentVersion

# TODO update the JSON string below
json = "{}"
# create an instance of AttachmentVersion from a JSON string
attachment_version_instance = AttachmentVersion.from_json(json)
# print the JSON string representation of the object
print(AttachmentVersion.to_json())

# convert the object into a dict
attachment_version_dict = attachment_version_instance.to_dict()
# create an instance of AttachmentVersion from a dict
attachment_version_from_dict = AttachmentVersion.from_dict(attachment_version_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


