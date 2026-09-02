# BalanceItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | **str** |  | 
**account_name** | **str** |  | 
**amount** | **str** |  | 

## Example

```python
from simplebilly_api.models.balance_item import BalanceItem

# TODO update the JSON string below
json = "{}"
# create an instance of BalanceItem from a JSON string
balance_item_instance = BalanceItem.from_json(json)
# print the JSON string representation of the object
print(BalanceItem.to_json())

# convert the object into a dict
balance_item_dict = balance_item_instance.to_dict()
# create an instance of BalanceItem from a dict
balance_item_from_dict = BalanceItem.from_dict(balance_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


