# ImportTestRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_key** | **str** |  | 
**provider** | **str** |  | 

## Example

```python
from simplebilly_api.models.import_test_request import ImportTestRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ImportTestRequest from a JSON string
import_test_request_instance = ImportTestRequest.from_json(json)
# print the JSON string representation of the object
print(ImportTestRequest.to_json())

# convert the object into a dict
import_test_request_dict = import_test_request_instance.to_dict()
# create an instance of ImportTestRequest from a dict
import_test_request_from_dict = ImportTestRequest.from_dict(import_test_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


