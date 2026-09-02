# PayrollMonth


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gross** | **str** |  | 
**month** | **int** |  | 
**net** | **str** |  | 

## Example

```python
from simplebilly_api.models.payroll_month import PayrollMonth

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollMonth from a JSON string
payroll_month_instance = PayrollMonth.from_json(json)
# print the JSON string representation of the object
print(PayrollMonth.to_json())

# convert the object into a dict
payroll_month_dict = payroll_month_instance.to_dict()
# create an instance of PayrollMonth from a dict
payroll_month_from_dict = PayrollMonth.from_dict(payroll_month_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


