# PayrollRunApi


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**approved_at** | **datetime** |  | [optional] 
**approved_by** | **UUID** |  | [optional] 
**created_at** | **datetime** |  | 
**entries** | [**List[PayrollEntryApi]**](PayrollEntryApi.md) |  | 
**month** | **int** |  | 
**payment_date** | **date** |  | [optional] 
**period_label** | **str** |  | 
**run_id** | **UUID** |  | 
**status** | [**PayrollRunStatus**](PayrollRunStatus.md) |  | 
**tenant_id** | **UUID** |  | 
**total_employee_count** | **int** |  | 
**total_employer_cost** | **str** |  | 
**total_gross** | **str** |  | 
**total_net** | **str** |  | 
**total_social_security** | **str** |  | 
**total_taxes** | **str** |  | 
**updated_at** | **datetime** |  | [optional] 
**year** | **int** |  | 

## Example

```python
from simplebilly_api.models.payroll_run_api import PayrollRunApi

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollRunApi from a JSON string
payroll_run_api_instance = PayrollRunApi.from_json(json)
# print the JSON string representation of the object
print(PayrollRunApi.to_json())

# convert the object into a dict
payroll_run_api_dict = payroll_run_api_instance.to_dict()
# create an instance of PayrollRunApi from a dict
payroll_run_api_from_dict = PayrollRunApi.from_dict(payroll_run_api_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


