# Automation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**automation_key** | **str** |  | 
**config** | **object** |  | 
**created_at** | **datetime** |  | 
**enabled** | **bool** |  | 
**last_run_at** | **datetime** |  | [optional] 
**next_run_at** | **datetime** |  | [optional] 
**tenant_id** | **UUID** |  | 
**updated_at** | **datetime** |  | 

## Example

```python
from simplebilly_api.models.automation import Automation

# TODO update the JSON string below
json = "{}"
# create an instance of Automation from a JSON string
automation_instance = Automation.from_json(json)
# print the JSON string representation of the object
print(Automation.to_json())

# convert the object into a dict
automation_dict = automation_instance.to_dict()
# create an instance of Automation from a dict
automation_from_dict = Automation.from_dict(automation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


