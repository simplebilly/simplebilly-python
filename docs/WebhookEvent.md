# WebhookEvent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attempts** | **int** |  | [optional] 
**channel** | **str** | source for inbound, target URL for outbound. | [optional] 
**direction** | [**WebhookDirection**](WebhookDirection.md) | inbound | outbound | 
**event_type** | **str** |  | 
**last_error** | **str** |  | [optional] 
**payload** | **object** |  | [optional] 
**status** | [**WebhookEventStatus**](WebhookEventStatus.md) | accepted | delivered | failed | [optional] 

## Example

```python
from simplebilly_api.models.webhook_event import WebhookEvent

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEvent from a JSON string
webhook_event_instance = WebhookEvent.from_json(json)
# print the JSON string representation of the object
print(WebhookEvent.to_json())

# convert the object into a dict
webhook_event_dict = webhook_event_instance.to_dict()
# create an instance of WebhookEvent from a dict
webhook_event_from_dict = WebhookEvent.from_dict(webhook_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


