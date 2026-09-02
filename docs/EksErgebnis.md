# EksErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gesamtergebnis** | **str** |  | 
**monate** | [**List[EksMonatsWert]**](EksMonatsWert.md) |  | 
**prognose_naechste_6_monate** | **str** |  | 
**summe_ausgaben** | **str** |  | 
**summe_einnahmen** | **str** |  | 
**zeitraum_bis** | **str** |  | 
**zeitraum_von** | **str** |  | 

## Example

```python
from simplebilly_api.models.eks_ergebnis import EksErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of EksErgebnis from a JSON string
eks_ergebnis_instance = EksErgebnis.from_json(json)
# print the JSON string representation of the object
print(EksErgebnis.to_json())

# convert the object into a dict
eks_ergebnis_dict = eks_ergebnis_instance.to_dict()
# create an instance of EksErgebnis from a dict
eks_ergebnis_from_dict = EksErgebnis.from_dict(eks_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


