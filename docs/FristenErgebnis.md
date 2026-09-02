# FristenErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**anzahl** | **int** |  | 
**fristen** | [**List[FristEintrag]**](FristEintrag.md) |  | 

## Example

```python
from simplebilly_api.models.fristen_ergebnis import FristenErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of FristenErgebnis from a JSON string
fristen_ergebnis_instance = FristenErgebnis.from_json(json)
# print the JSON string representation of the object
print(FristenErgebnis.to_json())

# convert the object into a dict
fristen_ergebnis_dict = fristen_ergebnis_instance.to_dict()
# create an instance of FristenErgebnis from a dict
fristen_ergebnis_from_dict = FristenErgebnis.from_dict(fristen_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


