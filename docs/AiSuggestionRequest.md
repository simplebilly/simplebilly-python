# AiSuggestionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**instructions** | **str** |  | [optional] 
**message_body** | **str** |  | [optional] 
**ticket_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.ai_suggestion_request import AiSuggestionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AiSuggestionRequest from a JSON string
ai_suggestion_request_instance = AiSuggestionRequest.from_json(json)
# print the JSON string representation of the object
print(AiSuggestionRequest.to_json())

# convert the object into a dict
ai_suggestion_request_dict = ai_suggestion_request_instance.to_dict()
# create an instance of AiSuggestionRequest from a dict
ai_suggestion_request_from_dict = AiSuggestionRequest.from_dict(ai_suggestion_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


