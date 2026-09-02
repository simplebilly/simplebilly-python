# FristEintrag


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bezeichnung** | **str** |  | 
**faellig** | **str** |  | 
**faellig_original** | **str** |  | 
**hinweis** | **str** |  | [optional] 
**typ** | **str** |  | 
**zeitraum** | **str** |  | 

## Example

```python
from simplebilly_api.models.frist_eintrag import FristEintrag

# TODO update the JSON string below
json = "{}"
# create an instance of FristEintrag from a JSON string
frist_eintrag_instance = FristEintrag.from_json(json)
# print the JSON string representation of the object
print(FristEintrag.to_json())

# convert the object into a dict
frist_eintrag_dict = frist_eintrag_instance.to_dict()
# create an instance of FristEintrag from a dict
frist_eintrag_from_dict = FristEintrag.from_dict(frist_eintrag_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


