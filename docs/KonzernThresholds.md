# KonzernThresholds


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bilanzsumme** | **str** |  | 
**mitarbeiter** | **int** |  | 
**netto_umsatz** | **str** |  | 

## Example

```python
from simplebilly_api.models.konzern_thresholds import KonzernThresholds

# TODO update the JSON string below
json = "{}"
# create an instance of KonzernThresholds from a JSON string
konzern_thresholds_instance = KonzernThresholds.from_json(json)
# print the JSON string representation of the object
print(KonzernThresholds.to_json())

# convert the object into a dict
konzern_thresholds_dict = konzern_thresholds_instance.to_dict()
# create an instance of KonzernThresholds from a dict
konzern_thresholds_from_dict = KonzernThresholds.from_dict(konzern_thresholds_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


