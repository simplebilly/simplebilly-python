# TargetProgress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**base_value** | **float** |  | 
**base_year** | **int** |  | 
**description** | **str** |  | 
**id** | **UUID** |  | 
**progress_pct** | **float** | Current year&#39;s emissions for the scope as % of the target. None when no data. | [optional] 
**scope** | **str** |  | 
**target_value** | **float** |  | 
**target_year** | **int** |  | 

## Example

```python
from simplebilly_api.models.target_progress import TargetProgress

# TODO update the JSON string below
json = "{}"
# create an instance of TargetProgress from a JSON string
target_progress_instance = TargetProgress.from_json(json)
# print the JSON string representation of the object
print(TargetProgress.to_json())

# convert the object into a dict
target_progress_dict = target_progress_instance.to_dict()
# create an instance of TargetProgress from a dict
target_progress_from_dict = TargetProgress.from_dict(target_progress_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


