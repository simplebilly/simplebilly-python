# EuerZeileDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**abschnitt** | **str** |  | 
**betrag_gesamt** | **str** |  | 
**bezeichnung** | **str** |  | 
**kategorien** | [**List[EuerKatSumme]**](EuerKatSumme.md) |  | 
**zeile** | **int** |  | 

## Example

```python
from simplebilly_api.models.euer_zeile_detail import EuerZeileDetail

# TODO update the JSON string below
json = "{}"
# create an instance of EuerZeileDetail from a JSON string
euer_zeile_detail_instance = EuerZeileDetail.from_json(json)
# print the JSON string representation of the object
print(EuerZeileDetail.to_json())

# convert the object into a dict
euer_zeile_detail_dict = euer_zeile_detail_instance.to_dict()
# create an instance of EuerZeileDetail from a dict
euer_zeile_detail_from_dict = EuerZeileDetail.from_dict(euer_zeile_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


