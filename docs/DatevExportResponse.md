# DatevExportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**booking_count** | **int** |  | 
**csv_content** | **str** |  | 
**filename** | **str** |  | 

## Example

```python
from simplebilly_api.models.datev_export_response import DatevExportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DatevExportResponse from a JSON string
datev_export_response_instance = DatevExportResponse.from_json(json)
# print the JSON string representation of the object
print(DatevExportResponse.to_json())

# convert the object into a dict
datev_export_response_dict = datev_export_response_instance.to_dict()
# create an instance of DatevExportResponse from a dict
datev_export_response_from_dict = DatevExportResponse.from_dict(datev_export_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


