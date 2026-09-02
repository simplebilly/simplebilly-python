# BudgetKategorie


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**budget** | **str** |  | 
**differenz** | **str** |  | 
**goal** | **str** | User-set monthly goal for the category, if any. | [optional] 
**ist** | **str** |  | 
**kategorie** | **str** |  | 

## Example

```python
from simplebilly_api.models.budget_kategorie import BudgetKategorie

# TODO update the JSON string below
json = "{}"
# create an instance of BudgetKategorie from a JSON string
budget_kategorie_instance = BudgetKategorie.from_json(json)
# print the JSON string representation of the object
print(BudgetKategorie.to_json())

# convert the object into a dict
budget_kategorie_dict = budget_kategorie_instance.to_dict()
# create an instance of BudgetKategorie from a dict
budget_kategorie_from_dict = BudgetKategorie.from_dict(budget_kategorie_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


