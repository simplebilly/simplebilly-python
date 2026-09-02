# EuerZeile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**abschnitt** | **str** |  | 
**betrag** | **str** |  | 
**bezeichnung** | **str** |  | 
**zeile** | **int** |  | 

## Example

```python
from simplebilly_api.models.euer_zeile import EuerZeile

# TODO update the JSON string below
json = "{}"
# create an instance of EuerZeile from a JSON string
euer_zeile_instance = EuerZeile.from_json(json)
# print the JSON string representation of the object
print(EuerZeile.to_json())

# convert the object into a dict
euer_zeile_dict = euer_zeile_instance.to_dict()
# create an instance of EuerZeile from a dict
euer_zeile_from_dict = EuerZeile.from_dict(euer_zeile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


