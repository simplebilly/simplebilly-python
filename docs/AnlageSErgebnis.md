# AnlageSErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gewinn_verlust** | **str** |  | 
**jahr** | **int** |  | 
**kfz_hinweise** | [**List[AnlageSKfzHinweis]**](AnlageSKfzHinweis.md) |  | 

## Example

```python
from simplebilly_api.models.anlage_s_ergebnis import AnlageSErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of AnlageSErgebnis from a JSON string
anlage_s_ergebnis_instance = AnlageSErgebnis.from_json(json)
# print the JSON string representation of the object
print(AnlageSErgebnis.to_json())

# convert the object into a dict
anlage_s_ergebnis_dict = anlage_s_ergebnis_instance.to_dict()
# create an instance of AnlageSErgebnis from a dict
anlage_s_ergebnis_from_dict = AnlageSErgebnis.from_dict(anlage_s_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


