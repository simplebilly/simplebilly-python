# WorkflowAction

One action inside a workflow. Only `email` is supported for now.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action_type** | **str** |  | 
**body** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.workflow_action import WorkflowAction

# TODO update the JSON string below
json = "{}"
# create an instance of WorkflowAction from a JSON string
workflow_action_instance = WorkflowAction.from_json(json)
# print the JSON string representation of the object
print(WorkflowAction.to_json())

# convert the object into a dict
workflow_action_dict = workflow_action_instance.to_dict()
# create an instance of WorkflowAction from a dict
workflow_action_from_dict = WorkflowAction.from_dict(workflow_action_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


