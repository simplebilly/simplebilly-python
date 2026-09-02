# KostenVorschau


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**eintraege** | [**List[KostenEintrag]**](KostenEintrag.md) |  | 
**gesamt** | **str** |  | 

## Example

```python
from simplebilly_api.models.kosten_vorschau import KostenVorschau

# TODO update the JSON string below
json = "{}"
# create an instance of KostenVorschau from a JSON string
kosten_vorschau_instance = KostenVorschau.from_json(json)
# print the JSON string representation of the object
print(KostenVorschau.to_json())

# convert the object into a dict
kosten_vorschau_dict = kosten_vorschau_instance.to_dict()
# create an instance of KostenVorschau from a dict
kosten_vorschau_from_dict = KostenVorschau.from_dict(kosten_vorschau_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


