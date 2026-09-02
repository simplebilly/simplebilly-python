# EksMonatsWert


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ausgaben** | **str** |  | 
**einnahmen** | **str** |  | 
**ergebnis** | **str** |  | 
**monat** | **str** |  | 

## Example

```python
from simplebilly_api.models.eks_monats_wert import EksMonatsWert

# TODO update the JSON string below
json = "{}"
# create an instance of EksMonatsWert from a JSON string
eks_monats_wert_instance = EksMonatsWert.from_json(json)
# print the JSON string representation of the object
print(EksMonatsWert.to_json())

# convert the object into a dict
eks_monats_wert_dict = eks_monats_wert_instance.to_dict()
# create an instance of EksMonatsWert from a dict
eks_monats_wert_from_dict = EksMonatsWert.from_dict(eks_monats_wert_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


