# Activity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activity_type** | [**ActivityType**](ActivityType.md) | One of: call | email | meeting | task | note | 
**assigned_to** | **str** | User responsible (&#x60;employee.employee_id&#x60;). | [optional] 
**contact_id** | **str** | Contact this activity belongs to (&#x60;contact.contact_id&#x60;). References the contact entity. | [optional] 
**description** | **str** |  | [optional] 
**due_date** | **date** | Follow-up / Wiedervorlage date. Open activities with a due date in the past are overdue. | [optional] 
**reminder_date** | **date** | When to remind about the follow-up. | [optional] 
**status** | [**ActivityStatus**](ActivityStatus.md) | One of: open | done | cancelled | 
**subject** | **str** | Short subject line. | 

## Example

```python
from simplebilly_api.models.activity import Activity

# TODO update the JSON string below
json = "{}"
# create an instance of Activity from a JSON string
activity_instance = Activity.from_json(json)
# print the JSON string representation of the object
print(Activity.to_json())

# convert the object into a dict
activity_dict = activity_instance.to_dict()
# create an instance of Activity from a dict
activity_from_dict = Activity.from_dict(activity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


