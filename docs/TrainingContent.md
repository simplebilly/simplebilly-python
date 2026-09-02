# TrainingContent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**contact** | [**ContactInfo**](ContactInfo.md) |  | 
**pass_score** | **int** |  | 
**quiz** | [**List[QuizQuestion]**](QuizQuestion.md) |  | 
**sections** | [**List[Section]**](Section.md) |  | 
**title** | **str** |  | 
**title_en** | **str** |  | 

## Example

```python
from simplebilly_api.models.training_content import TrainingContent

# TODO update the JSON string below
json = "{}"
# create an instance of TrainingContent from a JSON string
training_content_instance = TrainingContent.from_json(json)
# print the JSON string representation of the object
print(TrainingContent.to_json())

# convert the object into a dict
training_content_dict = training_content_instance.to_dict()
# create an instance of TrainingContent from a dict
training_content_from_dict = TrainingContent.from_dict(training_content_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


