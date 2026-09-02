# Employee


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **str** |  | [optional] 
**backup_employee_id** | **UUID** | References another employee who covers when this employee is absent. | [optional] 
**bic** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**country** | [**CountryCode**](CountryCode.md) |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**date_of_birth** | **date** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**department_id** | **UUID** | References the department entity. | [optional] 
**email** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**gender** | [**Gender**](Gender.md) | Gender for pay-transparency reporting: \&quot;male\&quot;, \&quot;female\&quot; or \&quot;diverse\&quot;. | [optional] 
**hire_date** | **date** |  | [optional] 
**hourly_cost** | **str** | Hourly cost rate in EUR for labor-cost reporting; when unset the rate is derived from &#x60;monthly_salary / (weekly_hours * 4.33)&#x60;. | [optional] 
**iban** | **str** |  | [optional] 
**id** | **UUID** |  | [optional] 
**job_title** | **str** |  | [optional] 
**last_login** | **datetime** |  | [optional] 
**last_name** | **str** |  | [optional] 
**last_updated** | **datetime** |  | [optional] 
**monthly_salary** | **str** | Gross monthly salary in EUR for pay-transparency reporting. | [optional] 
**phone** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**status** | [**EmployeeStatus**](EmployeeStatus.md) |  | [optional] 
**tenant_id** | **UUID** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**user_id** | **UUID** | References the user entity. | [optional] 
**weekly_hours** | **str** | Contractual weekly working hours for pay-transparency normalization. | [optional] 
**zip** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.employee import Employee

# TODO update the JSON string below
json = "{}"
# create an instance of Employee from a JSON string
employee_instance = Employee.from_json(json)
# print the JSON string representation of the object
print(Employee.to_json())

# convert the object into a dict
employee_dict = employee_instance.to_dict()
# create an instance of Employee from a dict
employee_from_dict = Employee.from_dict(employee_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


