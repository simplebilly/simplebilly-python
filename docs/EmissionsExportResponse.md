# EmissionsExportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**csv_content** | **str** |  | 
**filename** | **str** |  | 

## Example

```python
from simplebilly_api.models.emissions_export_response import EmissionsExportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EmissionsExportResponse from a JSON string
emissions_export_response_instance = EmissionsExportResponse.from_json(json)
# print the JSON string representation of the object
print(EmissionsExportResponse.to_json())

# convert the object into a dict
emissions_export_response_dict = emissions_export_response_instance.to_dict()
# create an instance of EmissionsExportResponse from a dict
emissions_export_response_from_dict = EmissionsExportResponse.from_dict(emissions_export_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


