# KostenEintrag


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**beschreibung** | **str** |  | 
**betrag** | **str** |  | 
**datum** | **str** |  | 
**typ** | **str** |  | 

## Example

```python
from simplebilly_api.models.kosten_eintrag import KostenEintrag

# TODO update the JSON string below
json = "{}"
# create an instance of KostenEintrag from a JSON string
kosten_eintrag_instance = KostenEintrag.from_json(json)
# print the JSON string representation of the object
print(KostenEintrag.to_json())

# convert the object into a dict
kosten_eintrag_dict = kosten_eintrag_instance.to_dict()
# create an instance of KostenEintrag from a dict
kosten_eintrag_from_dict = KostenEintrag.from_dict(kosten_eintrag_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


