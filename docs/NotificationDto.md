# NotificationDto

Wire shape of a notification row (mirrors frontend Notification type).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | 
**id** | **UUID** |  | 
**is_read** | **bool** |  | 
**message** | **str** |  | [optional] 
**sent_via_email** | **bool** |  | 
**tenant_id** | **UUID** |  | 
**title** | **str** |  | 
**user_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.notification_dto import NotificationDto

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationDto from a JSON string
notification_dto_instance = NotificationDto.from_json(json)
# print the JSON string representation of the object
print(NotificationDto.to_json())

# convert the object into a dict
notification_dto_dict = notification_dto_instance.to_dict()
# create an instance of NotificationDto from a dict
notification_dto_from_dict = NotificationDto.from_dict(notification_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


