# RecurringTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **str** |  | [readonly] 
**deleted_at** | **str** |  | [optional] [readonly] 
**end_date** | **date** |  | [optional] 
**execution_interval** | **str** |  | 
**execution_status** | **str** |  | 
**finalize** | **bool** |  | 
**last_executed_at** | **datetime** |  | [optional] 
**name** | **str** |  | 
**next_execution_at** | **datetime** |  | [optional] 
**start_date** | **date** |  | 
**template_id** | **str** |  | 
**template_type** | **str** |  | 
**updated_at** | **str** |  | [optional] [readonly] 
**voucher_data** | **object** |  | 

## Example

```python
from simplebilly_api.models.recurring_template import RecurringTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of RecurringTemplate from a JSON string
recurring_template_instance = RecurringTemplate.from_json(json)
# print the JSON string representation of the object
print(RecurringTemplate.to_json())

# convert the object into a dict
recurring_template_dict = recurring_template_instance.to_dict()
# create an instance of RecurringTemplate from a dict
recurring_template_from_dict = RecurringTemplate.from_dict(recurring_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


