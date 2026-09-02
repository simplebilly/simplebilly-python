# ImportTestResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | **str** |  | [optional] 
**ok** | **bool** |  | 

## Example

```python
from simplebilly_api.models.import_test_response import ImportTestResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ImportTestResponse from a JSON string
import_test_response_instance = ImportTestResponse.from_json(json)
# print the JSON string representation of the object
print(ImportTestResponse.to_json())

# convert the object into a dict
import_test_response_dict = import_test_response_instance.to_dict()
# create an instance of ImportTestResponse from a dict
import_test_response_from_dict = ImportTestResponse.from_dict(import_test_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


