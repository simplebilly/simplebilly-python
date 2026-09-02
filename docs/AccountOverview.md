# AccountOverview


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | **str** |  | 
**account_name** | **str** |  | 
**balance** | **str** |  | 
**credit_total** | **str** |  | 
**debit_total** | **str** |  | 

## Example

```python
from simplebilly_api.models.account_overview import AccountOverview

# TODO update the JSON string below
json = "{}"
# create an instance of AccountOverview from a JSON string
account_overview_instance = AccountOverview.from_json(json)
# print the JSON string representation of the object
print(AccountOverview.to_json())

# convert the object into a dict
account_overview_dict = account_overview_instance.to_dict()
# create an instance of AccountOverview from a dict
account_overview_from_dict = AccountOverview.from_dict(account_overview_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


