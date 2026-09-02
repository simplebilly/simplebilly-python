# PlanLimits

Per-plan numeric limits. `-1` in any field means unlimited.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**max_connectors** | **int** |  | 
**max_invoices_per_month** | **int** |  | 
**max_users** | **int** |  | 
**metered** | **Dict[str, int]** |  | [optional] 
**paid_connectors** | **List[str]** | Connectors that are *not* included in this plan (require a higher tier). Empty &#x3D; all connectors included on this plan. | 

## Example

```python
from simplebilly_api.models.plan_limits import PlanLimits

# TODO update the JSON string below
json = "{}"
# create an instance of PlanLimits from a JSON string
plan_limits_instance = PlanLimits.from_json(json)
# print the JSON string representation of the object
print(PlanLimits.to_json())

# convert the object into a dict
plan_limits_dict = plan_limits_instance.to_dict()
# create an instance of PlanLimits from a dict
plan_limits_from_dict = PlanLimits.from_dict(plan_limits_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


