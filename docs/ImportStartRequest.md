# ImportStartRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_key** | **str** |  | 
**provider** | **str** |  | 
**years** | **List[int]** |  | 

## Example

```python
from simplebilly_api.models.import_start_request import ImportStartRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ImportStartRequest from a JSON string
import_start_request_instance = ImportStartRequest.from_json(json)
# print the JSON string representation of the object
print(ImportStartRequest.to_json())

# convert the object into a dict
import_start_request_dict = import_start_request_instance.to_dict()
# create an instance of ImportStartRequest from a dict
import_start_request_from_dict = ImportStartRequest.from_dict(import_start_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


