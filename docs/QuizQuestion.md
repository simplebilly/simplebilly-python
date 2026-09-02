# QuizQuestion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**options** | **List[str]** |  | 
**options_en** | **List[str]** |  | 
**question** | **str** |  | 
**question_en** | **str** |  | 

## Example

```python
from simplebilly_api.models.quiz_question import QuizQuestion

# TODO update the JSON string below
json = "{}"
# create an instance of QuizQuestion from a JSON string
quiz_question_instance = QuizQuestion.from_json(json)
# print the JSON string representation of the object
print(QuizQuestion.to_json())

# convert the object into a dict
quiz_question_dict = quiz_question_instance.to_dict()
# create an instance of QuizQuestion from a dict
quiz_question_from_dict = QuizQuestion.from_dict(quiz_question_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


