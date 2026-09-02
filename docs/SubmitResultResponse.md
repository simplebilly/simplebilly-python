# SubmitResultResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**certificate_id** | **str** |  | [optional] 
**completion_id** | **UUID** |  | 
**pass_score** | **int** |  | 
**passed** | **bool** |  | 
**score** | **int** |  | 
**valid_until** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.submit_result_response import SubmitResultResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubmitResultResponse from a JSON string
submit_result_response_instance = SubmitResultResponse.from_json(json)
# print the JSON string representation of the object
print(SubmitResultResponse.to_json())

# convert the object into a dict
submit_result_response_dict = submit_result_response_instance.to_dict()
# create an instance of SubmitResultResponse from a dict
submit_result_response_from_dict = SubmitResultResponse.from_dict(submit_result_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


