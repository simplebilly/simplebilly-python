# TrainingAssignmentCreate


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
from simplebilly_api.models.training_assignment_create import TrainingAssignmentCreate

# TODO update the JSON string below
json = "{}"
# create an instance of TrainingAssignmentCreate from a JSON string
training_assignment_create_instance = TrainingAssignmentCreate.from_json(json)
# print the JSON string representation of the object
print(TrainingAssignmentCreate.to_json())

# convert the object into a dict
training_assignment_create_dict = training_assignment_create_instance.to_dict()
# create an instance of TrainingAssignmentCreate from a dict
training_assignment_create_from_dict = TrainingAssignmentCreate.from_dict(training_assignment_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


