# QuotaOverview


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**features** | [**PlanFeatures**](PlanFeatures.md) |  | 
**is_trialing** | **bool** |  | 
**limits** | [**PlanLimits**](PlanLimits.md) |  | 
**metered** | [**List[MeteredUsage]**](MeteredUsage.md) |  | 
**plan** | **str** |  | 
**plan_name** | **str** |  | 
**trial_ends_at** | **datetime** |  | [optional] 
**usage** | [**UsageSnapshot**](UsageSnapshot.md) |  | 

## Example

```python
from simplebilly_api.models.quota_overview import QuotaOverview

# TODO update the JSON string below
json = "{}"
# create an instance of QuotaOverview from a JSON string
quota_overview_instance = QuotaOverview.from_json(json)
# print the JSON string representation of the object
print(QuotaOverview.to_json())

# convert the object into a dict
quota_overview_dict = quota_overview_instance.to_dict()
# create an instance of QuotaOverview from a dict
quota_overview_from_dict = QuotaOverview.from_dict(quota_overview_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


