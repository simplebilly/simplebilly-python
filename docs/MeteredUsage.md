# MeteredUsage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**limit** | **int** |  | 
**meter** | **str** |  | 
**used** | **int** |  | 

## Example

```python
from simplebilly_api.models.metered_usage import MeteredUsage

# TODO update the JSON string below
json = "{}"
# create an instance of MeteredUsage from a JSON string
metered_usage_instance = MeteredUsage.from_json(json)
# print the JSON string representation of the object
print(MeteredUsage.to_json())

# convert the object into a dict
metered_usage_dict = metered_usage_instance.to_dict()
# create an instance of MeteredUsage from a dict
metered_usage_from_dict = MeteredUsage.from_dict(metered_usage_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


