# RecurringTemplateUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**end_date** | **date** |  | [optional] 
**execution_interval** | **str** |  | [optional] 
**execution_status** | [**ExecutionStatus**](ExecutionStatus.md) |  | [optional] 
**finalize** | **bool** |  | [optional] 
**last_executed_at** | **datetime** |  | [optional] 
**name** | **str** |  | [optional] 
**next_execution_at** | **datetime** |  | [optional] 
**start_date** | **date** |  | [optional] 
**template_type** | [**RecurringTemplateType**](RecurringTemplateType.md) |  | [optional] 
**voucher_data** | **object** |  | [optional] 

## Example

```python
from simplebilly_api.models.recurring_template_update import RecurringTemplateUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of RecurringTemplateUpdate from a JSON string
recurring_template_update_instance = RecurringTemplateUpdate.from_json(json)
# print the JSON string representation of the object
print(RecurringTemplateUpdate.to_json())

# convert the object into a dict
recurring_template_update_dict = recurring_template_update_instance.to_dict()
# create an instance of RecurringTemplateUpdate from a dict
recurring_template_update_from_dict = RecurringTemplateUpdate.from_dict(recurring_template_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


