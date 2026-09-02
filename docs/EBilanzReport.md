# EBilanzReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_overview** | [**List[AccountOverview]**](AccountOverview.md) |  | 
**balance_sheet** | [**BalanceSheet**](BalanceSheet.md) |  | 
**generated_at** | **str** |  | 
**income_statement** | [**IncomeStatement**](IncomeStatement.md) |  | 
**period** | **str** |  | 
**vat_summary** | [**VatSummary**](VatSummary.md) |  | 

## Example

```python
from simplebilly_api.models.e_bilanz_report import EBilanzReport

# TODO update the JSON string below
json = "{}"
# create an instance of EBilanzReport from a JSON string
e_bilanz_report_instance = EBilanzReport.from_json(json)
# print the JSON string representation of the object
print(EBilanzReport.to_json())

# convert the object into a dict
e_bilanz_report_dict = e_bilanz_report_instance.to_dict()
# create an instance of EBilanzReport from a dict
e_bilanz_report_from_dict = EBilanzReport.from_dict(e_bilanz_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


