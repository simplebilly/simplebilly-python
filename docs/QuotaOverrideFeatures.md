# QuotaOverrideFeatures


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**erp** | **bool** |  | [optional] 
**fancy_reports** | **bool** |  | [optional] 
**tax_automations** | **bool** |  | [optional] 

## Example

```python
from simplebilly_api.models.quota_override_features import QuotaOverrideFeatures

# TODO update the JSON string below
json = "{}"
# create an instance of QuotaOverrideFeatures from a JSON string
quota_override_features_instance = QuotaOverrideFeatures.from_json(json)
# print the JSON string representation of the object
print(QuotaOverrideFeatures.to_json())

# convert the object into a dict
quota_override_features_dict = quota_override_features_instance.to_dict()
# create an instance of QuotaOverrideFeatures from a dict
quota_override_features_from_dict = QuotaOverrideFeatures.from_dict(quota_override_features_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


