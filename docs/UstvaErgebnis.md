# UstvaErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bis** | **str** |  | 
**hinweis** | **str** |  | [optional] 
**ist_kleinunternehmer** | **bool** |  | 
**kz_41** | **str** |  | 
**kz_43** | **str** |  | 
**kz_46** | **str** |  | 
**kz_47** | **str** |  | 
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
**von** | **str** |  | 
**zahllast** | **str** |  | 
**zeitraum** | **str** |  | 
**zeitraum_typ** | **str** |  | 

## Example

```python
from simplebilly_api.models.ustva_ergebnis import UstvaErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of UstvaErgebnis from a JSON string
ustva_ergebnis_instance = UstvaErgebnis.from_json(json)
# print the JSON string representation of the object
print(UstvaErgebnis.to_json())

# convert the object into a dict
ustva_ergebnis_dict = ustva_ergebnis_instance.to_dict()
# create an instance of UstvaErgebnis from a dict
ustva_ergebnis_from_dict = UstvaErgebnis.from_dict(ustva_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


