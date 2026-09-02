# GdprBillingInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_period_end** | **datetime** |  | [optional] 
**current_period_start** | **datetime** |  | [optional] 
**plan** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**tenant_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.gdpr_billing_info import GdprBillingInfo

# TODO update the JSON string below
json = "{}"
# create an instance of GdprBillingInfo from a JSON string
gdpr_billing_info_instance = GdprBillingInfo.from_json(json)
# print the JSON string representation of the object
print(GdprBillingInfo.to_json())

# convert the object into a dict
gdpr_billing_info_dict = gdpr_billing_info_instance.to_dict()
# create an instance of GdprBillingInfo from a dict
gdpr_billing_info_from_dict = GdprBillingInfo.from_dict(gdpr_billing_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


