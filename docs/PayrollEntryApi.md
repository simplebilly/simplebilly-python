# PayrollEntryApi


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**av_employee** | **str** |  | 
**av_employer** | **str** |  | 
**church_tax_amount** | **str** |  | 
**employee** | [**Employee**](Employee.md) |  | [optional] 
**employee_id** | **UUID** |  | 
**entry_id** | **UUID** |  | 
**extra_payment_reason** | **str** |  | [optional] 
**extra_payments** | **str** |  | 
**gross_salary** | **str** |  | 
**kv_employee** | **str** |  | 
**kv_employer** | **str** |  | 
**lohnsteuer** | **str** |  | 
**net_salary** | **str** |  | 
**notes** | **str** |  | [optional] 
**pv_employee** | **str** |  | 
**pv_employer** | **str** |  | 
**run_id** | **UUID** |  | 
**rv_employee** | **str** |  | 
**rv_employer** | **str** |  | 
**sick_days** | **int** |  | 
**soli** | **str** |  | 
**status** | [**PayrollRunStatus**](PayrollRunStatus.md) |  | 
**total_deductions** | **str** |  | 
**total_employer_cost** | **str** |  | 
**vacation_days_used** | **int** |  | 

## Example

```python
from simplebilly_api.models.payroll_entry_api import PayrollEntryApi

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollEntryApi from a JSON string
payroll_entry_api_instance = PayrollEntryApi.from_json(json)
# print the JSON string representation of the object
print(PayrollEntryApi.to_json())

# convert the object into a dict
payroll_entry_api_dict = payroll_entry_api_instance.to_dict()
# create an instance of PayrollEntryApi from a dict
payroll_entry_api_from_dict = PayrollEntryApi.from_dict(payroll_entry_api_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


