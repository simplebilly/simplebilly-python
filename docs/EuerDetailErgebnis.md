# EuerDetailErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**jahr** | **int** |  | 
**zeilen** | [**List[EuerZeileDetail]**](EuerZeileDetail.md) |  | 

## Example

```python
from simplebilly_api.models.euer_detail_ergebnis import EuerDetailErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of EuerDetailErgebnis from a JSON string
euer_detail_ergebnis_instance = EuerDetailErgebnis.from_json(json)
# print the JSON string representation of the object
print(EuerDetailErgebnis.to_json())

# convert the object into a dict
euer_detail_ergebnis_dict = euer_detail_ergebnis_instance.to_dict()
# create an instance of EuerDetailErgebnis from a dict
euer_detail_ergebnis_from_dict = EuerDetailErgebnis.from_dict(euer_detail_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


