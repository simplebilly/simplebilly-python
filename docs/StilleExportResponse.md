# StilleExportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**csv_content** | **str** |  | 
**filename** | **str** |  | 

## Example

```python
from simplebilly_api.models.stille_export_response import StilleExportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of StilleExportResponse from a JSON string
stille_export_response_instance = StilleExportResponse.from_json(json)
# print the JSON string representation of the object
print(StilleExportResponse.to_json())

# convert the object into a dict
stille_export_response_dict = stille_export_response_instance.to_dict()
# create an instance of StilleExportResponse from a dict
stille_export_response_from_dict = StilleExportResponse.from_dict(stille_export_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


