# QuotaOverride

Schema of the `tenants.quotas` JSON override column. Any field that is present overrides the plan-derived value.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**features** | [**QuotaOverrideFeatures**](QuotaOverrideFeatures.md) |  | [optional] 
**max_connectors** | **int** |  | [optional] 
**max_invoices_per_month** | **int** |  | [optional] 
**max_users** | **int** |  | [optional] 
**metered** | **Dict[str, int]** |  | [optional] 
**plan** | **str** | Custom plan id; unknown ids resolve to enterprise limits. | [optional] 

## Example

```python
from simplebilly_api.models.quota_override import QuotaOverride

# TODO update the JSON string below
json = "{}"
# create an instance of QuotaOverride from a JSON string
quota_override_instance = QuotaOverride.from_json(json)
# print the JSON string representation of the object
print(QuotaOverride.to_json())

# convert the object into a dict
quota_override_dict = quota_override_instance.to_dict()
# create an instance of QuotaOverride from a dict
quota_override_from_dict = QuotaOverride.from_dict(quota_override_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


