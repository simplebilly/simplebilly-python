# DatevImportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count** | **int** |  | 
**filename** | **str** |  | 
**rows** | [**List[DatevImportRow]**](DatevImportRow.md) |  | 

## Example

```python
from simplebilly_api.models.datev_import_response import DatevImportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DatevImportResponse from a JSON string
datev_import_response_instance = DatevImportResponse.from_json(json)
# print the JSON string representation of the object
print(DatevImportResponse.to_json())

# convert the object into a dict
datev_import_response_dict = datev_import_response_instance.to_dict()
# create an instance of DatevImportResponse from a dict
datev_import_response_from_dict = DatevImportResponse.from_dict(datev_import_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


