# ContactHistoryResponse

Aggregated history for a single contact: all communications plus a lightweight per-channel breakdown.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **str** |  | 
**inbound_count** | **int** |  | 
**items** | [**List[CustomerCommunication]**](CustomerCommunication.md) |  | 
**outbound_count** | **int** |  | 

## Example

```python
from simplebilly_api.models.contact_history_response import ContactHistoryResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ContactHistoryResponse from a JSON string
contact_history_response_instance = ContactHistoryResponse.from_json(json)
# print the JSON string representation of the object
print(ContactHistoryResponse.to_json())

# convert the object into a dict
contact_history_response_dict = contact_history_response_instance.to_dict()
# create an instance of ContactHistoryResponse from a dict
contact_history_response_from_dict = ContactHistoryResponse.from_dict(contact_history_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


