# YearlyPayrollSummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**avg_employee_count** | **int** |  | 
**months** | [**List[PayrollSummaryItem]**](PayrollSummaryItem.md) |  | 
**year** | **int** |  | 
**yearly_employer_cost** | **str** |  | 
**yearly_gross** | **str** |  | 
**yearly_net** | **str** |  | 

## Example

```python
from simplebilly_api.models.yearly_payroll_summary import YearlyPayrollSummary

# TODO update the JSON string below
json = "{}"
# create an instance of YearlyPayrollSummary from a JSON string
yearly_payroll_summary_instance = YearlyPayrollSummary.from_json(json)
# print the JSON string representation of the object
print(YearlyPayrollSummary.to_json())

# convert the object into a dict
yearly_payroll_summary_dict = yearly_payroll_summary_instance.to_dict()
# create an instance of YearlyPayrollSummary from a dict
yearly_payroll_summary_from_dict = YearlyPayrollSummary.from_dict(yearly_payroll_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


