# AutomationDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**automation_key** | **str** |  | 
**config** | **object** |  | 
**default_day** | **int** |  | [optional] 
**description** | **str** |  | 
**enabled** | **bool** |  | 
**kind** | **str** |  | 
**last_run_at** | **datetime** |  | [optional] 
**next_run_at** | **datetime** |  | [optional] 
**schedule_kind** | **str** |  | 

## Example

```python
from simplebilly_api.models.automation_dto import AutomationDto

# TODO update the JSON string below
json = "{}"
# create an instance of AutomationDto from a JSON string
automation_dto_instance = AutomationDto.from_json(json)
# print the JSON string representation of the object
print(AutomationDto.to_json())

# convert the object into a dict
automation_dto_dict = automation_dto_instance.to_dict()
# create an instance of AutomationDto from a dict
automation_dto_from_dict = AutomationDto.from_dict(automation_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


