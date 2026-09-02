# TimelineEvent

Single timeline entry aggregated from the contact's activity across all related modules (communications, quotations, orders, invoices, documents).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **str** | RFC3339 UTC timestamp for sorting. | 
**detail** | **str** |  | [optional] 
**id** | **str** | Source record id (stringified). | 
**status** | **str** |  | [optional] 
**title** | **str** |  | 
**type** | **str** | Source module: communication | quotation | order | invoice | attachment. | 

## Example

```python
from simplebilly_api.models.timeline_event import TimelineEvent

# TODO update the JSON string below
json = "{}"
# create an instance of TimelineEvent from a JSON string
timeline_event_instance = TimelineEvent.from_json(json)
# print the JSON string representation of the object
print(TimelineEvent.to_json())

# convert the object into a dict
timeline_event_dict = timeline_event_instance.to_dict()
# create an instance of TimelineEvent from a dict
timeline_event_from_dict = TimelineEvent.from_dict(timeline_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


