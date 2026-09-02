# RecurringTemplateCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**end_date** | **date** |  | [optional] 
**execution_interval** | **str** |  | 
**execution_status** | [**ExecutionStatus**](ExecutionStatus.md) |  | 
**finalize** | **bool** |  | [optional] 
**last_executed_at** | **datetime** |  | [optional] 
**name** | **str** |  | 
**next_execution_at** | **datetime** |  | [optional] 
**start_date** | **date** |  | 
**template_type** | [**RecurringTemplateType**](RecurringTemplateType.md) |  | 
**voucher_data** | **object** |  | [optional] 

## Example

```python
from simplebilly_api.models.recurring_template_create import RecurringTemplateCreate

# TODO update the JSON string below
json = "{}"
# create an instance of RecurringTemplateCreate from a JSON string
recurring_template_create_instance = RecurringTemplateCreate.from_json(json)
# print the JSON string representation of the object
print(RecurringTemplateCreate.to_json())

# convert the object into a dict
recurring_template_create_dict = recurring_template_create_instance.to_dict()
# create an instance of RecurringTemplateCreate from a dict
recurring_template_create_from_dict = RecurringTemplateCreate.from_dict(recurring_template_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


