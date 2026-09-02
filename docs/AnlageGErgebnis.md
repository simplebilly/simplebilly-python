# AnlageGErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gewinn_verlust** | **str** |  | 
**gewst_gezahlt** | **str** |  | 
**gewst_messbetrag_approx** | **str** |  | 
**gewst_pflichtig** | **bool** |  | 
**jahr** | **int** |  | 
**kfz_hinweise** | [**List[AnlageGKfzHinweis]**](AnlageGKfzHinweis.md) |  | 

## Example

```python
from simplebilly_api.models.anlage_g_ergebnis import AnlageGErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of AnlageGErgebnis from a JSON string
anlage_g_ergebnis_instance = AnlageGErgebnis.from_json(json)
# print the JSON string representation of the object
print(AnlageGErgebnis.to_json())

# convert the object into a dict
anlage_g_ergebnis_dict = anlage_g_ergebnis_instance.to_dict()
# create an instance of AnlageGErgebnis from a dict
anlage_g_ergebnis_from_dict = AnlageGErgebnis.from_dict(anlage_g_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


