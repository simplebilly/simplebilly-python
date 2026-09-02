# NewVersionRequest

Body for uploading a new version. Bytes must already be stored under `file_name` via the object storage API.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_name** | **str** | Storage key of the already-uploaded bytes. | 
**file_size** | **int** |  | [optional] 
**mime_type** | **str** |  | [optional] 
**original_name** | **str** |  | [optional] 
**sha256_hash** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.new_version_request import NewVersionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of NewVersionRequest from a JSON string
new_version_request_instance = NewVersionRequest.from_json(json)
# print the JSON string representation of the object
print(NewVersionRequest.to_json())

# convert the object into a dict
new_version_request_dict = new_version_request_instance.to_dict()
# create an instance of NewVersionRequest from a dict
new_version_request_from_dict = NewVersionRequest.from_dict(new_version_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


