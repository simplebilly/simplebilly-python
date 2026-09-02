# PlanFeatures

Feature flags per plan.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connectors** | **bool** |  | 
**erp** | **bool** |  | 
**fancy_reports** | **bool** |  | 
**tax_automations** | **bool** |  | 

## Example

```python
from simplebilly_api.models.plan_features import PlanFeatures

# TODO update the JSON string below
json = "{}"
# create an instance of PlanFeatures from a JSON string
plan_features_instance = PlanFeatures.from_json(json)
# print the JSON string representation of the object
print(PlanFeatures.to_json())

# convert the object into a dict
plan_features_dict = plan_features_instance.to_dict()
# create an instance of PlanFeatures from a dict
plan_features_from_dict = PlanFeatures.from_dict(plan_features_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


