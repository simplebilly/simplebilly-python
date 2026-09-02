# Plan

One canonical plan. `price_eur == -1.0` means custom pricing.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**features** | [**PlanFeatures**](PlanFeatures.md) |  | 
**id** | **str** |  | 
**limits** | [**PlanLimits**](PlanLimits.md) |  | 
**name** | **str** |  | 
**price_eur** | **float** |  | 

## Example

```python
from simplebilly_api.models.plan import Plan

# TODO update the JSON string below
json = "{}"
# create an instance of Plan from a JSON string
plan_instance = Plan.from_json(json)
# print the JSON string representation of the object
print(Plan.to_json())

# convert the object into a dict
plan_dict = plan_instance.to_dict()
# create an instance of Plan from a dict
plan_from_dict = Plan.from_dict(plan_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


