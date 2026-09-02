# ExpenseItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** |  | 
**category** | **str** |  | 
**percentage** | **float** |  | 

## Example

```python
from simplebilly_api.models.expense_item import ExpenseItem

# TODO update the JSON string below
json = "{}"
# create an instance of ExpenseItem from a JSON string
expense_item_instance = ExpenseItem.from_json(json)
# print the JSON string representation of the object
print(ExpenseItem.to_json())

# convert the object into a dict
expense_item_dict = expense_item_instance.to_dict()
# create an instance of ExpenseItem from a dict
expense_item_from_dict = ExpenseItem.from_dict(expense_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


