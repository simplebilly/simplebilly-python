# TrainingAssignmentUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assigned_by** | **UUID** |  | [optional] 
**due_date** | **date** |  | [optional] 
**employee_id** | **UUID** |  | [optional] 
**notes** | **str** |  | [optional] 
**status** | [**AssignmentStatus**](AssignmentStatus.md) |  | [optional] 
**training_id** | **UUID** |  | [optional] 

## Example

```python
from simplebilly_api.models.training_assignment_update import TrainingAssignmentUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of TrainingAssignmentUpdate from a JSON string
training_assignment_update_instance = TrainingAssignmentUpdate.from_json(json)
# print the JSON string representation of the object
print(TrainingAssignmentUpdate.to_json())

# convert the object into a dict
training_assignment_update_dict = training_assignment_update_instance.to_dict()
# create an instance of TrainingAssignmentUpdate from a dict
training_assignment_update_from_dict = TrainingAssignmentUpdate.from_dict(training_assignment_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


