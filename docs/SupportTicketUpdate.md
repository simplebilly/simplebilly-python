# SupportTicketUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assigned_to** | **UUID** |  | [optional] 
**channel_id** | **UUID** |  | [optional] 
**channel_type** | [**SupportChannelType**](SupportChannelType.md) |  | [optional] 
**closed_at** | **datetime** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**customer_email** | **str** |  | [optional] 
**customer_id** | **str** | References the customer entity. | [optional] 
**customer_name** | **str** |  | [optional] 
**external_id** | **str** |  | [optional] 
**first_message_at** | **datetime** |  | [optional] 
**last_message_at** | **datetime** |  | [optional] 
**lead_id** | **UUID** | References the lead entity. | [optional] 
**message_count** | **int** |  | [optional] 
**order_ref** | **str** |  | [optional] 
**priority** | [**TicketPriority**](TicketPriority.md) |  | [optional] 
**resolution** | **str** |  | [optional] 
**status** | [**SupportTicketStatus**](SupportTicketStatus.md) |  | [optional] 
**subject** | **str** |  | [optional] 
**tags** | **object** |  | [optional] 
**tenant_id** | **UUID** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.support_ticket_update import SupportTicketUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of SupportTicketUpdate from a JSON string
support_ticket_update_instance = SupportTicketUpdate.from_json(json)
# print the JSON string representation of the object
print(SupportTicketUpdate.to_json())

# convert the object into a dict
support_ticket_update_dict = support_ticket_update_instance.to_dict()
# create an instance of SupportTicketUpdate from a dict
support_ticket_update_from_dict = SupportTicketUpdate.from_dict(support_ticket_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


