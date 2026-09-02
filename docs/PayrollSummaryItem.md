# PayrollSummaryItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**employee_count** | **int** |  | 
**month** | **str** |  | 
**status** | [**PayrollRunStatus**](PayrollRunStatus.md) |  | 
**total_employer_cost** | **str** |  | 
**total_gross** | **str** |  | 
**total_net** | **str** |  | 
**year** | **int** |  | 

## Example

```python
from simplebilly_api.models.payroll_summary_item import PayrollSummaryItem

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollSummaryItem from a JSON string
payroll_summary_item_instance = PayrollSummaryItem.from_json(json)
# print the JSON string representation of the object
print(PayrollSummaryItem.to_json())

# convert the object into a dict
payroll_summary_item_dict = payroll_summary_item_instance.to_dict()
# create an instance of PayrollSummaryItem from a dict
payroll_summary_item_from_dict = PayrollSummaryItem.from_dict(payroll_summary_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


