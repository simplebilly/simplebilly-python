# SubmitResultDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**answers** | **List[int]** | Selected answer indices (required for scored builtin trainings). | 
**assignment_id** | **UUID** |  | [optional] 
**score** | **int** | Score 0–100. Only trusted for plugin trainings without server-side scoring; builtin trainings are always re-scored from &#x60;answers&#x60;. | 
**training_code** | **str** |  | 

## Example

```python
from simplebilly_api.models.submit_result_dto import SubmitResultDto

# TODO update the JSON string below
json = "{}"
# create an instance of SubmitResultDto from a JSON string
submit_result_dto_instance = SubmitResultDto.from_json(json)
# print the JSON string representation of the object
print(SubmitResultDto.to_json())

# convert the object into a dict
submit_result_dto_dict = submit_result_dto_instance.to_dict()
# create an instance of SubmitResultDto from a dict
submit_result_dto_from_dict = SubmitResultDto.from_dict(submit_result_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


