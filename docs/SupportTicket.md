# SupportTicket


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assigned_to** | **UUID** |  | [optional] 
**channel_id** | **UUID** |  | [optional] 
**channel_type** | [**SupportChannelType**](SupportChannelType.md) |  | [optional] 
**closed_at** | **datetime** |  | [optional] 
**created_at** | **datetime** |  | 
**customer_email** | **str** |  | [optional] 
**customer_id** | **str** | References the customer entity. | [optional] 
**customer_name** | **str** |  | [optional] 
**external_id** | **str** |  | [optional] 
**first_message_at** | **datetime** |  | 
**last_message_at** | **datetime** |  | 
**lead_id** | **UUID** | References the lead entity. | [optional] 
**message_count** | **int** |  | 
**order_ref** | **str** |  | [optional] 
**priority** | [**TicketPriority**](TicketPriority.md) |  | 
**resolution** | **str** |  | [optional] 
**status** | [**SupportTicketStatus**](SupportTicketStatus.md) |  | 
**subject** | **str** |  | 
**tags** | **object** |  | 
**tenant_id** | **UUID** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.support_ticket import SupportTicket

# TODO update the JSON string below
json = "{}"
# create an instance of SupportTicket from a JSON string
support_ticket_instance = SupportTicket.from_json(json)
# print the JSON string representation of the object
print(SupportTicket.to_json())

# convert the object into a dict
support_ticket_dict = support_ticket_instance.to_dict()
# create an instance of SupportTicket from a dict
support_ticket_from_dict = SupportTicket.from_dict(support_ticket_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


