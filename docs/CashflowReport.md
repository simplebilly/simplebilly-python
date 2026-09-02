# CashflowReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**closing_balance** | **float** |  | 
**financing_cashflow** | **float** |  | 
**investing_cashflow** | **float** |  | 
**net_cashflow** | **float** |  | 
**opening_balance** | **float** |  | 
**operating_cashflow** | **float** |  | 
**period** | **str** |  | 

## Example

```python
from simplebilly_api.models.cashflow_report import CashflowReport

# TODO update the JSON string below
json = "{}"
# create an instance of CashflowReport from a JSON string
cashflow_report_instance = CashflowReport.from_json(json)
# print the JSON string representation of the object
print(CashflowReport.to_json())

# convert the object into a dict
cashflow_report_dict = cashflow_report_instance.to_dict()
# create an instance of CashflowReport from a dict
cashflow_report_from_dict = CashflowReport.from_dict(cashflow_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


