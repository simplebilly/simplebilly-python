# BWAExpenses


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**expense_breakdown** | [**List[ExpenseItem]**](ExpenseItem.md) |  | 
**total_expenses** | **str** |  | 

## Example

```python
from simplebilly_api.models.bwa_expenses import BWAExpenses

# TODO update the JSON string below
json = "{}"
# create an instance of BWAExpenses from a JSON string
bwa_expenses_instance = BWAExpenses.from_json(json)
# print the JSON string representation of the object
print(BWAExpenses.to_json())

# convert the object into a dict
bwa_expenses_dict = bwa_expenses_instance.to_dict()
# create an instance of BWAExpenses from a dict
bwa_expenses_from_dict = BWAExpenses.from_dict(bwa_expenses_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


