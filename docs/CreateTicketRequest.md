# CreateTicketRequest

Request body for creating a support ticket. Wraps the generated `SupportTicketCreateDto` fields plus `message_body` which is not a Model field (used to create the initial `ticket_message`).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **UUID** |  | [optional] 
**channel_type** | **str** |  | [optional] 
**customer_email** | **str** |  | [optional] 
**customer_id** | **str** |  | [optional] 
**customer_name** | **str** |  | [optional] 
**external_id** | **str** |  | [optional] 
**message_body** | **str** |  | 
**order_ref** | **str** |  | [optional] 
**subject** | **str** |  | 

## Example

```python
from simplebilly_api.models.create_ticket_request import CreateTicketRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTicketRequest from a JSON string
create_ticket_request_instance = CreateTicketRequest.from_json(json)
# print the JSON string representation of the object
print(CreateTicketRequest.to_json())

# convert the object into a dict
create_ticket_request_dict = create_ticket_request_instance.to_dict()
# create an instance of CreateTicketRequest from a dict
create_ticket_request_from_dict = CreateTicketRequest.from_dict(create_ticket_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


