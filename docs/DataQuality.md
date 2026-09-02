# DataQuality


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activity_lines** | **int** |  | 
**activity_share_pct** | **float** |  | 
**spend_lines** | **int** |  | 

## Example

```python
from simplebilly_api.models.data_quality import DataQuality

# TODO update the JSON string below
json = "{}"
# create an instance of DataQuality from a JSON string
data_quality_instance = DataQuality.from_json(json)
# print the JSON string representation of the object
print(DataQuality.to_json())

# convert the object into a dict
data_quality_dict = data_quality_instance.to_dict()
# create an instance of DataQuality from a dict
data_quality_from_dict = DataQuality.from_dict(data_quality_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


