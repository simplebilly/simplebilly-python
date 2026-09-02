# ApiResponseGdprExport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ApiResponseGdprExportData**](ApiResponseGdprExportData.md) |  | [optional] 
**error** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.api_response_gdpr_export import ApiResponseGdprExport

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseGdprExport from a JSON string
api_response_gdpr_export_instance = ApiResponseGdprExport.from_json(json)
# print the JSON string representation of the object
print(ApiResponseGdprExport.to_json())

# convert the object into a dict
api_response_gdpr_export_dict = api_response_gdpr_export_instance.to_dict()
# create an instance of ApiResponseGdprExport from a dict
api_response_gdpr_export_from_dict = ApiResponseGdprExport.from_dict(api_response_gdpr_export_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


