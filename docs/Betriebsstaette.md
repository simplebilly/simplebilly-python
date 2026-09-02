# Betriebsstaette

Eine Betriebsstätte mit der Anzahl der sozialversicherungspflichtig Beschäftigten (Jahresdurchschnitt des Vorjahres).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**beschaefigte** | **int** |  | 
**name** | **str** |  | 

## Example

```python
from simplebilly_api.models.betriebsstaette import Betriebsstaette

# TODO update the JSON string below
json = "{}"
# create an instance of Betriebsstaette from a JSON string
betriebsstaette_instance = Betriebsstaette.from_json(json)
# print the JSON string representation of the object
print(Betriebsstaette.to_json())

# convert the object into a dict
betriebsstaette_dict = betriebsstaette_instance.to_dict()
# create an instance of Betriebsstaette from a dict
betriebsstaette_from_dict = Betriebsstaette.from_dict(betriebsstaette_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


