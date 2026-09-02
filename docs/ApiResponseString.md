# ApiResponseString


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | **str** |  | [optional] 
**error** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.api_response_string import ApiResponseString

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseString from a JSON string
api_response_string_instance = ApiResponseString.from_json(json)
# print the JSON string representation of the object
print(ApiResponseString.to_json())

# convert the object into a dict
api_response_string_dict = api_response_string_instance.to_dict()
# create an instance of ApiResponseString from a dict
api_response_string_from_dict = ApiResponseString.from_dict(api_response_string_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


