# TicketMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**author_email** | **str** |  | [optional] 
**author_name** | **str** |  | [optional] 
**body** | **str** |  | 
**body_html** | **str** |  | [optional] 
**channel_id** | **UUID** |  | [optional] 
**created_at** | **datetime** |  | 
**direction** | [**MessageDirection**](MessageDirection.md) |  | 
**external_id** | **str** |  | [optional] 
**is_internal** | **bool** |  | 
**message_type** | [**MessageType**](MessageType.md) |  | 
**metadata** | **object** |  | 
**tenant_id** | **UUID** |  | 
**ticket_id** | **UUID** | References the ticket entity. | 

## Example

```python
from simplebilly_api.models.ticket_message import TicketMessage

# TODO update the JSON string below
json = "{}"
# create an instance of TicketMessage from a JSON string
ticket_message_instance = TicketMessage.from_json(json)
# print the JSON string representation of the object
print(TicketMessage.to_json())

# convert the object into a dict
ticket_message_dict = ticket_message_instance.to_dict()
# create an instance of TicketMessage from a dict
ticket_message_from_dict = TicketMessage.from_dict(ticket_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


