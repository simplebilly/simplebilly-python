# GoBDExportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**booking_count** | **int** |  | 
**csv_content** | **str** |  | 
**filename** | **str** |  | 

## Example

```python
from simplebilly_api.models.go_bd_export_response import GoBDExportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GoBDExportResponse from a JSON string
go_bd_export_response_instance = GoBDExportResponse.from_json(json)
# print the JSON string representation of the object
print(GoBDExportResponse.to_json())

# convert the object into a dict
go_bd_export_response_dict = go_bd_export_response_instance.to_dict()
# create an instance of GoBDExportResponse from a dict
go_bd_export_response_from_dict = GoBDExportResponse.from_dict(go_bd_export_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


