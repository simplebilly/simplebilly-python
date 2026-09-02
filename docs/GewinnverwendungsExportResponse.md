# GewinnverwendungsExportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**csv_content** | **str** |  | 
**filename** | **str** |  | 

## Example

```python
from simplebilly_api.models.gewinnverwendungs_export_response import GewinnverwendungsExportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GewinnverwendungsExportResponse from a JSON string
gewinnverwendungs_export_response_instance = GewinnverwendungsExportResponse.from_json(json)
# print the JSON string representation of the object
print(GewinnverwendungsExportResponse.to_json())

# convert the object into a dict
gewinnverwendungs_export_response_dict = gewinnverwendungs_export_response_instance.to_dict()
# create an instance of GewinnverwendungsExportResponse from a dict
gewinnverwendungs_export_response_from_dict = GewinnverwendungsExportResponse.from_dict(gewinnverwendungs_export_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


