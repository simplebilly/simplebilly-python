# EuerErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**anlage_zugaenge** | **str** |  | 
**gewinn_verlust** | **str** |  | 
**jahr** | **int** |  | 
**summe_ausgaben** | **str** |  | 
**summe_einnahmen** | **str** |  | 
**zeilen** | [**List[EuerZeile]**](EuerZeile.md) |  | 

## Example

```python
from simplebilly_api.models.euer_ergebnis import EuerErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of EuerErgebnis from a JSON string
euer_ergebnis_instance = EuerErgebnis.from_json(json)
# print the JSON string representation of the object
print(EuerErgebnis.to_json())

# convert the object into a dict
euer_ergebnis_dict = euer_ergebnis_instance.to_dict()
# create an instance of EuerErgebnis from a dict
euer_ergebnis_from_dict = EuerErgebnis.from_dict(euer_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


