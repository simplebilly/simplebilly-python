# GdprActivity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action** | **str** |  | 
**created_at** | **datetime** |  | 
**description** | **str** |  | [optional] 
**id** | **UUID** |  | 
**tenant_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.gdpr_activity import GdprActivity

# TODO update the JSON string below
json = "{}"
# create an instance of GdprActivity from a JSON string
gdpr_activity_instance = GdprActivity.from_json(json)
# print the JSON string representation of the object
print(GdprActivity.to_json())

# convert the object into a dict
gdpr_activity_dict = gdpr_activity_instance.to_dict()
# create an instance of GdprActivity from a dict
gdpr_activity_from_dict = GdprActivity.from_dict(gdpr_activity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


