# CustomerCommunication


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**body** | **str** | The message body, call summary or note text. | [optional] 
**channel** | [**CommunicationChannel**](CommunicationChannel.md) |  | 
**contact_id** | **str** | The contact (customer/supplier) this communication belongs to. References the contact entity. | 
**counterparty** | **str** | Email/phone of the counterparty, if applicable. | [optional] 
**direction** | [**CommunicationDirection**](CommunicationDirection.md) |  | 
**occurred_at** | **datetime** | When the communication happened (defaults to now on create). | [optional] 
**subject** | **str** |  | [optional] 
**tags** | **object** | Free-form tags, e.g. &#x60;[\&quot;follow-up-required\&quot;]&#x60;. | [optional] 

## Example

```python
from simplebilly_api.models.customer_communication import CustomerCommunication

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerCommunication from a JSON string
customer_communication_instance = CustomerCommunication.from_json(json)
# print the JSON string representation of the object
print(CustomerCommunication.to_json())

# convert the object into a dict
customer_communication_dict = customer_communication_instance.to_dict()
# create an instance of CustomerCommunication from a dict
customer_communication_from_dict = CustomerCommunication.from_dict(customer_communication_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


