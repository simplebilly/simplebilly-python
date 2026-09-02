# GdprNotification


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | 
**id** | **UUID** |  | 
**is_read** | **bool** |  | 
**message** | **str** |  | [optional] 
**tenant_id** | **UUID** |  | 
**title** | **str** |  | 

## Example

```python
from simplebilly_api.models.gdpr_notification import GdprNotification

# TODO update the JSON string below
json = "{}"
# create an instance of GdprNotification from a JSON string
gdpr_notification_instance = GdprNotification.from_json(json)
# print the JSON string representation of the object
print(GdprNotification.to_json())

# convert the object into a dict
gdpr_notification_dict = gdpr_notification_instance.to_dict()
# create an instance of GdprNotification from a dict
gdpr_notification_from_dict = GdprNotification.from_dict(gdpr_notification_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


