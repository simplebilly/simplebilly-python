# TrainingAssignment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assigned_by** | **UUID** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**due_date** | **date** |  | [optional] 
**employee_id** | **UUID** |  | [optional] 
**id** | **UUID** |  | [optional] 
**notes** | **str** |  | [optional] 
**status** | [**AssignmentStatus**](AssignmentStatus.md) |  | [optional] 
**tenant_id** | **UUID** |  | [optional] 
**training_id** | **UUID** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.training_assignment import TrainingAssignment

# TODO update the JSON string below
json = "{}"
# create an instance of TrainingAssignment from a JSON string
training_assignment_instance = TrainingAssignment.from_json(json)
# print the JSON string representation of the object
print(TrainingAssignment.to_json())

# convert the object into a dict
training_assignment_dict = training_assignment_instance.to_dict()
# create an instance of TrainingAssignment from a dict
training_assignment_from_dict = TrainingAssignment.from_dict(training_assignment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


