# IncomeStatement


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**expense_items** | [**List[PnLItem]**](PnLItem.md) |  | 
**net_income** | **str** |  | 
**revenue_items** | [**List[PnLItem]**](PnLItem.md) |  | 
**total_expenses** | **str** |  | 
**total_revenue** | **str** |  | 

## Example

```python
from simplebilly_api.models.income_statement import IncomeStatement

# TODO update the JSON string below
json = "{}"
# create an instance of IncomeStatement from a JSON string
income_statement_instance = IncomeStatement.from_json(json)
# print the JSON string representation of the object
print(IncomeStatement.to_json())

# convert the object into a dict
income_statement_dict = income_statement_instance.to_dict()
# create an instance of IncomeStatement from a dict
income_statement_from_dict = IncomeStatement.from_dict(income_statement_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


