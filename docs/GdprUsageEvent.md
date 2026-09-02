# GdprUsageEvent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | 
**event_type** | **str** |  | 
**id** | **UUID** |  | 
**quantity** | **int** |  | 
**tenant_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.gdpr_usage_event import GdprUsageEvent

# TODO update the JSON string below
json = "{}"
# create an instance of GdprUsageEvent from a JSON string
gdpr_usage_event_instance = GdprUsageEvent.from_json(json)
# print the JSON string representation of the object
print(GdprUsageEvent.to_json())

# convert the object into a dict
gdpr_usage_event_dict = gdpr_usage_event_instance.to_dict()
# create an instance of GdprUsageEvent from a dict
gdpr_usage_event_from_dict = GdprUsageEvent.from_dict(gdpr_usage_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


