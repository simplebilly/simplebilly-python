# PlausibilitySummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**errors** | **int** |  | 
**overall_status** | [**CheckStatus**](CheckStatus.md) |  | 
**passed** | **int** |  | 
**total_checks** | **int** |  | 
**warnings** | **int** |  | 

## Example

```python
from simplebilly_api.models.plausibility_summary import PlausibilitySummary

# TODO update the JSON string below
json = "{}"
# create an instance of PlausibilitySummary from a JSON string
plausibility_summary_instance = PlausibilitySummary.from_json(json)
# print the JSON string representation of the object
print(PlausibilitySummary.to_json())

# convert the object into a dict
plausibility_summary_dict = plausibility_summary_instance.to_dict()
# create an instance of PlausibilitySummary from a dict
plausibility_summary_from_dict = PlausibilitySummary.from_dict(plausibility_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


