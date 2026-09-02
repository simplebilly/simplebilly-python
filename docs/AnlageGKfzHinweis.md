# AnlageGKfzHinweis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bezeichnung** | **str** |  | 
**kennzeichen** | **str** |  | 
**privat_anteil_prozent** | **str** |  | 

## Example

```python
from simplebilly_api.models.anlage_g_kfz_hinweis import AnlageGKfzHinweis

# TODO update the JSON string below
json = "{}"
# create an instance of AnlageGKfzHinweis from a JSON string
anlage_g_kfz_hinweis_instance = AnlageGKfzHinweis.from_json(json)
# print the JSON string representation of the object
print(AnlageGKfzHinweis.to_json())

# convert the object into a dict
anlage_g_kfz_hinweis_dict = anlage_g_kfz_hinweis_instance.to_dict()
# create an instance of AnlageGKfzHinweis from a dict
anlage_g_kfz_hinweis_from_dict = AnlageGKfzHinweis.from_dict(anlage_g_kfz_hinweis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


