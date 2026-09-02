# ContactTimelineResponse

Aggregated per-contact timeline.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **str** |  | 
**events** | [**List[TimelineEvent]**](TimelineEvent.md) |  | 

## Example

```python
from simplebilly_api.models.contact_timeline_response import ContactTimelineResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ContactTimelineResponse from a JSON string
contact_timeline_response_instance = ContactTimelineResponse.from_json(json)
# print the JSON string representation of the object
print(ContactTimelineResponse.to_json())

# convert the object into a dict
contact_timeline_response_dict = contact_timeline_response_instance.to_dict()
# create an instance of ContactTimelineResponse from a dict
contact_timeline_response_from_dict = ContactTimelineResponse.from_dict(contact_timeline_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


