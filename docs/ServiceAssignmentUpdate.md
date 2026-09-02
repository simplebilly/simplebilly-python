# ServiceAssignmentUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**employee_id** | **UUID** | References the employees entity. | [optional] 
**job_id** | **UUID** | References the service_jobs entity. | [optional] 
**notes** | **str** |  | [optional] 
**scheduled_date** | **date** | Work day the assignment is scheduled for. | [optional] 
**scheduled_end** | **str** | Planned end time of the assignment. | [optional] 
**scheduled_start** | **str** | Planned start time of the assignment. | [optional] 
**status** | [**ServiceAssignmentStatus**](ServiceAssignmentStatus.md) | Assignment lifecycle status: \&quot;planned\&quot;, \&quot;confirmed\&quot;, \&quot;en_route\&quot;, \&quot;in_progress\&quot;, \&quot;completed\&quot; or \&quot;cancelled\&quot;. | [optional] 

## Example

```python
from simplebilly_api.models.service_assignment_update import ServiceAssignmentUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ServiceAssignmentUpdate from a JSON string
service_assignment_update_instance = ServiceAssignmentUpdate.from_json(json)
# print the JSON string representation of the object
print(ServiceAssignmentUpdate.to_json())

# convert the object into a dict
service_assignment_update_dict = service_assignment_update_instance.to_dict()
# create an instance of ServiceAssignmentUpdate from a dict
service_assignment_update_from_dict = ServiceAssignmentUpdate.from_dict(service_assignment_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


