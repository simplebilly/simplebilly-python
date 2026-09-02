# TimeEntryClockOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**clock_out** | **datetime** |  | 
**hours** | **str** | Optional manual hours; when absent, derived from clock_in..clock_out. | [optional] 

## Example

```python
from simplebilly_api.models.time_entry_clock_out import TimeEntryClockOut

# TODO update the JSON string below
json = "{}"
# create an instance of TimeEntryClockOut from a JSON string
time_entry_clock_out_instance = TimeEntryClockOut.from_json(json)
# print the JSON string representation of the object
print(TimeEntryClockOut.to_json())

# convert the object into a dict
time_entry_clock_out_dict = time_entry_clock_out_instance.to_dict()
# create an instance of TimeEntryClockOut from a dict
time_entry_clock_out_from_dict = TimeEntryClockOut.from_dict(time_entry_clock_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


