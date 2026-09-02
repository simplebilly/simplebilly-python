# MarketplaceWebhookEvent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connection_id** | **str** | References the marketplace connection entity. | 
**event_body** | **object** |  | [optional] 
**event_type** | **str** |  | 
**headers** | **object** |  | [optional] 
**platform** | **str** |  | 
**processed** | **bool** |  | [optional] 
**processing_error** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.marketplace_webhook_event import MarketplaceWebhookEvent

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhookEvent from a JSON string
marketplace_webhook_event_instance = MarketplaceWebhookEvent.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhookEvent.to_json())

# convert the object into a dict
marketplace_webhook_event_dict = marketplace_webhook_event_instance.to_dict()
# create an instance of MarketplaceWebhookEvent from a dict
marketplace_webhook_event_from_dict = MarketplaceWebhookEvent.from_dict(marketplace_webhook_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


