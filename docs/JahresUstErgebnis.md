# JahresUstErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bis** | **str** |  | 
**gespeicherte_perioden** | **int** |  | 
**hat_ig_transaktionen** | **bool** |  | 
**ist_kleinunternehmer** | **bool** |  | 
**jahr** | **int** |  | 
**kz_41** | **str** |  | 
**kz_43** | **str** |  | 
**kz_46** | **str** |  | 
**kz_47** | **str** |  | 
**kz_48** | **str** |  | 
**kz_61** | **str** |  | 
**kz_66** | **str** |  | 
**kz_67** | **str** |  | 
**kz_81** | **str** |  | 
**kz_83** | **str** |  | 
**kz_84** | **str** |  | 
**kz_85** | **str** |  | 
**kz_86** | **str** |  | 
**kz_88** | **str** |  | 
**kz_89** | **str** |  | 
**kz_93** | **str** |  | 
**restschuld** | **str** |  | 
**summe_vorauszahlungen** | **str** |  | 
**von** | **str** |  | 
**zahllast** | **str** |  | 

## Example

```python
from simplebilly_api.models.jahres_ust_ergebnis import JahresUstErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of JahresUstErgebnis from a JSON string
jahres_ust_ergebnis_instance = JahresUstErgebnis.from_json(json)
# print the JSON string representation of the object
print(JahresUstErgebnis.to_json())

# convert the object into a dict
jahres_ust_ergebnis_dict = jahres_ust_ergebnis_instance.to_dict()
# create an instance of JahresUstErgebnis from a dict
jahres_ust_ergebnis_from_dict = JahresUstErgebnis.from_dict(jahres_ust_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


