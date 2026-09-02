# ActivityUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activity_type** | [**ActivityType**](ActivityType.md) | One of: call | email | meeting | task | note | [optional] 
**assigned_to** | **str** | User responsible (&#x60;employee.employee_id&#x60;). | [optional] 
**contact_id** | **str** | Contact this activity belongs to (&#x60;contact.contact_id&#x60;). References the contact entity. | [optional] 
**description** | **str** |  | [optional] 
**due_date** | **date** | Follow-up / Wiedervorlage date. Open activities with a due date in the past are overdue. | [optional] 
**reminder_date** | **date** | When to remind about the follow-up. | [optional] 
**status** | [**ActivityStatus**](ActivityStatus.md) | One of: open | done | cancelled | [optional] 
**subject** | **str** | Short subject line. | [optional] 

## Example

```python
from simplebilly_api.models.activity_update import ActivityUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ActivityUpdate from a JSON string
activity_update_instance = ActivityUpdate.from_json(json)
# print the JSON string representation of the object
print(ActivityUpdate.to_json())

# convert the object into a dict
activity_update_dict = activity_update_instance.to_dict()
# create an instance of ActivityUpdate from a dict
activity_update_from_dict = ActivityUpdate.from_dict(activity_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


