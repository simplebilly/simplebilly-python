# KstErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gesamt** | **str** |  | 
**gesamtbelastung** | **str** |  | 
**gewerbesteuer** | **str** |  | 
**gewinn** | **str** |  | 
**ist_kapitalgesellschaft** | **bool** |  | 
**jahr** | **int** |  | 
**koerperschaftsteuer** | **str** |  | 
**solidaritaetszuschlag** | **str** |  | 

## Example

```python
from simplebilly_api.models.kst_ergebnis import KstErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of KstErgebnis from a JSON string
kst_ergebnis_instance = KstErgebnis.from_json(json)
# print the JSON string representation of the object
print(KstErgebnis.to_json())

# convert the object into a dict
kst_ergebnis_dict = kst_ergebnis_instance.to_dict()
# create an instance of KstErgebnis from a dict
kst_ergebnis_from_dict = KstErgebnis.from_dict(kst_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


