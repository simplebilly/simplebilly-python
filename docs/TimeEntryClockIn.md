# TimeEntryClockIn


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**notes** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.time_entry_clock_in import TimeEntryClockIn

# TODO update the JSON string below
json = "{}"
# create an instance of TimeEntryClockIn from a JSON string
time_entry_clock_in_instance = TimeEntryClockIn.from_json(json)
# print the JSON string representation of the object
print(TimeEntryClockIn.to_json())

# convert the object into a dict
time_entry_clock_in_dict = time_entry_clock_in_instance.to_dict()
# create an instance of TimeEntryClockIn from a dict
time_entry_clock_in_from_dict = TimeEntryClockIn.from_dict(time_entry_clock_in_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


