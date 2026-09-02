# PayrollSummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first_name** | **str** |  | 
**hourly_gross** | **str** |  | [optional] 
**id** | **UUID** |  | 
**job_title** | **str** |  | 
**last_name** | **str** |  | 
**monthly_salary** | **str** |  | [optional] 
**months** | [**List[PayrollMonth]**](PayrollMonth.md) |  | 
**weekly_hours** | **str** |  | [optional] 
**year** | **int** |  | 

## Example

```python
from simplebilly_api.models.payroll_summary import PayrollSummary

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollSummary from a JSON string
payroll_summary_instance = PayrollSummary.from_json(json)
# print the JSON string representation of the object
print(PayrollSummary.to_json())

# convert the object into a dict
payroll_summary_dict = payroll_summary_instance.to_dict()
# create an instance of PayrollSummary from a dict
payroll_summary_from_dict = PayrollSummary.from_dict(payroll_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


