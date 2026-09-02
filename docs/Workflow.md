# Workflow


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**actions** | **object** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**name** | **str** |  | 
**trigger_event** | **str** | Event that triggers the workflow, e.g. &#x60;order.paid&#x60;, &#x60;order.shipped&#x60;. | 

## Example

```python
from simplebilly_api.models.workflow import Workflow

# TODO update the JSON string below
json = "{}"
# create an instance of Workflow from a JSON string
workflow_instance = Workflow.from_json(json)
# print the JSON string representation of the object
print(Workflow.to_json())

# convert the object into a dict
workflow_dict = workflow_instance.to_dict()
# create an instance of Workflow from a dict
workflow_from_dict = Workflow.from_dict(workflow_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


