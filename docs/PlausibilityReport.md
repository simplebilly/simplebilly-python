# PlausibilityReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**checks** | [**List[PlausibilityCheck]**](PlausibilityCheck.md) |  | 
**generated_at** | **str** |  | 
**summary** | [**PlausibilitySummary**](PlausibilitySummary.md) |  | 

## Example

```python
from simplebilly_api.models.plausibility_report import PlausibilityReport

# TODO update the JSON string below
json = "{}"
# create an instance of PlausibilityReport from a JSON string
plausibility_report_instance = PlausibilityReport.from_json(json)
# print the JSON string representation of the object
print(PlausibilityReport.to_json())

# convert the object into a dict
plausibility_report_dict = plausibility_report_instance.to_dict()
# create an instance of PlausibilityReport from a dict
plausibility_report_from_dict = PlausibilityReport.from_dict(plausibility_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


