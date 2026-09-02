# CustomerCommunicationUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**body** | **str** | The message body, call summary or note text. | [optional] 
**channel** | [**CommunicationChannel**](CommunicationChannel.md) |  | [optional] 
**contact_id** | **str** | The contact (customer/supplier) this communication belongs to. References the contact entity. | [optional] 
**counterparty** | **str** | Email/phone of the counterparty, if applicable. | [optional] 
**direction** | [**CommunicationDirection**](CommunicationDirection.md) |  | [optional] 
**occurred_at** | **datetime** | When the communication happened (defaults to now on create). | [optional] 
**subject** | **str** |  | [optional] 
**tags** | **object** | Free-form tags, e.g. &#x60;[\&quot;follow-up-required\&quot;]&#x60;. | [optional] 

## Example

```python
from simplebilly_api.models.customer_communication_update import CustomerCommunicationUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerCommunicationUpdate from a JSON string
customer_communication_update_instance = CustomerCommunicationUpdate.from_json(json)
# print the JSON string representation of the object
print(CustomerCommunicationUpdate.to_json())

# convert the object into a dict
customer_communication_update_dict = customer_communication_update_instance.to_dict()
# create an instance of CustomerCommunicationUpdate from a dict
customer_communication_update_from_dict = CustomerCommunicationUpdate.from_dict(customer_communication_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


