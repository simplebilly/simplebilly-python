# GewerbesteuerErgebnis


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**freibetrag** | **str** |  | 
**gesamtbelastung** | **str** |  | 
**gewerbeertrag** | **str** |  | 
**hebesatz** | **str** |  | 
**jahr** | **int** |  | 
**koerperschaftsteuer** | **str** |  | 
**land** | **str** |  | 
**messbetrag** | **str** |  | 
**steuer** | **str** |  | 
**steuer_art** | **str** |  | 

## Example

```python
from simplebilly_api.models.gewerbesteuer_ergebnis import GewerbesteuerErgebnis

# TODO update the JSON string below
json = "{}"
# create an instance of GewerbesteuerErgebnis from a JSON string
gewerbesteuer_ergebnis_instance = GewerbesteuerErgebnis.from_json(json)
# print the JSON string representation of the object
print(GewerbesteuerErgebnis.to_json())

# convert the object into a dict
gewerbesteuer_ergebnis_dict = gewerbesteuer_ergebnis_instance.to_dict()
# create an instance of GewerbesteuerErgebnis from a dict
gewerbesteuer_ergebnis_from_dict = GewerbesteuerErgebnis.from_dict(gewerbesteuer_ergebnis_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


