# AiSuggestion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**confidence** | **float** |  | 
**reasoning** | **str** |  | 
**suggested_priority** | **str** |  | [optional] 
**suggested_reply** | **str** |  | 
**suggested_status** | **str** |  | [optional] 
**tool_calls** | **List[str]** |  | 

## Example

```python
from simplebilly_api.models.ai_suggestion import AiSuggestion

# TODO update the JSON string below
json = "{}"
# create an instance of AiSuggestion from a JSON string
ai_suggestion_instance = AiSuggestion.from_json(json)
# print the JSON string representation of the object
print(AiSuggestion.to_json())

# convert the object into a dict
ai_suggestion_dict = ai_suggestion_instance.to_dict()
# create an instance of AiSuggestion from a dict
ai_suggestion_from_dict = AiSuggestion.from_dict(ai_suggestion_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


