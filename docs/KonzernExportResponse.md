# KonzernExportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**csv_content** | **str** |  | 
**filename** | **str** |  | 

## Example

```python
from simplebilly_api.models.konzern_export_response import KonzernExportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of KonzernExportResponse from a JSON string
konzern_export_response_instance = KonzernExportResponse.from_json(json)
# print the JSON string representation of the object
print(KonzernExportResponse.to_json())

# convert the object into a dict
konzern_export_response_dict = konzern_export_response_instance.to_dict()
# create an instance of KonzernExportResponse from a dict
konzern_export_response_from_dict = KonzernExportResponse.from_dict(konzern_export_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


