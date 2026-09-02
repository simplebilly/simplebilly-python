# QuartileBand


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**female_share_pct** | **float** |  | 
**hourly_median** | **str** |  | 
**male_share_pct** | **float** |  | 
**quartile** | **str** |  | 

## Example

```python
from simplebilly_api.models.quartile_band import QuartileBand

# TODO update the JSON string below
json = "{}"
# create an instance of QuartileBand from a JSON string
quartile_band_instance = QuartileBand.from_json(json)
# print the JSON string representation of the object
print(QuartileBand.to_json())

# convert the object into a dict
quartile_band_dict = quartile_band_instance.to_dict()
# create an instance of QuartileBand from a dict
quartile_band_from_dict = QuartileBand.from_dict(quartile_band_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


