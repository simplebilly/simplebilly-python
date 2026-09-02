# BudgetErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**jahr** | **int** |  | 
**monat** | **int** |  | 
**monats_budget** | [**List[BudgetKategorie]**](BudgetKategorie.md) |  | 
**prognose_restjahr** | [**List[BudgetKategorie]**](BudgetKategorie.md) |  | 

## Example

```python
from simplebilly_api.models.budget_ergebnis import BudgetErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of BudgetErgebnis from a JSON string
budget_ergebnis_instance = BudgetErgebnis.from_json(json)
# print the JSON string representation of the object
print(BudgetErgebnis.to_json())

# convert the object into a dict
budget_ergebnis_dict = budget_ergebnis_instance.to_dict()
# create an instance of BudgetErgebnis from a dict
budget_ergebnis_from_dict = BudgetErgebnis.from_dict(budget_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


