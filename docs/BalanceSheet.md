# BalanceSheet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assets** | [**List[BalanceItem]**](BalanceItem.md) |  | 
**balanced** | **bool** |  | 
**equity_liabilities** | [**List[BalanceItem]**](BalanceItem.md) |  | 
**total_assets** | **str** |  | 
**total_equity_liabilities** | **str** |  | 

## Example

```python
from simplebilly_api.models.balance_sheet import BalanceSheet

# TODO update the JSON string below
json = "{}"
# create an instance of BalanceSheet from a JSON string
balance_sheet_instance = BalanceSheet.from_json(json)
# print the JSON string representation of the object
print(BalanceSheet.to_json())

# convert the object into a dict
balance_sheet_dict = balance_sheet_instance.to_dict()
# create an instance of BalanceSheet from a dict
balance_sheet_from_dict = BalanceSheet.from_dict(balance_sheet_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


