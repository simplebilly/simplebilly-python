# UpdateAutomation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config** | **object** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from simplebilly_api.models.update_automation import UpdateAutomation

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateAutomation from a JSON string
update_automation_instance = UpdateAutomation.from_json(json)
# print the JSON string representation of the object
print(UpdateAutomation.to_json())

# convert the object into a dict
update_automation_dict = update_automation_instance.to_dict()
# create an instance of UpdateAutomation from a dict
update_automation_from_dict = UpdateAutomation.from_dict(update_automation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


