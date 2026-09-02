# WebhookSubscription


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_type** | **str** | Event type to react to (e.g. \&quot;order.created\&quot;); \&quot;*\&quot; &#x3D; all events. | 
**is_active** | **bool** |  | [optional] 
**name** | **str** | Human label (e.g. \&quot;Warehouse app\&quot;). | 
**secret** | **str** | Shared secret for HMAC-SHA256 signature, sent as X-Signature. | 
**url** | **str** |  | 

## Example

```python
from simplebilly_api.models.webhook_subscription import WebhookSubscription

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookSubscription from a JSON string
webhook_subscription_instance = WebhookSubscription.from_json(json)
# print the JSON string representation of the object
print(WebhookSubscription.to_json())

# convert the object into a dict
webhook_subscription_dict = webhook_subscription_instance.to_dict()
# create an instance of WebhookSubscription from a dict
webhook_subscription_from_dict = WebhookSubscription.from_dict(webhook_subscription_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


