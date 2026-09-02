# GewinnverwendungsZeile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**betrag** | **str** | Betrag in EUR (2 Nachkommastellen, als String formatiert). | 
**label** | **str** | Deutsche Bezeichnung der Zeile. | 

## Example

```python
from simplebilly_api.models.gewinnverwendungs_zeile import GewinnverwendungsZeile

# TODO update the JSON string below
json = "{}"
# create an instance of GewinnverwendungsZeile from a JSON string
gewinnverwendungs_zeile_instance = GewinnverwendungsZeile.from_json(json)
# print the JSON string representation of the object
print(GewinnverwendungsZeile.to_json())

# convert the object into a dict
gewinnverwendungs_zeile_dict = gewinnverwendungs_zeile_instance.to_dict()
# create an instance of GewinnverwendungsZeile from a dict
gewinnverwendungs_zeile_from_dict = GewinnverwendungsZeile.from_dict(gewinnverwendungs_zeile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


