# TimeEntryDto

API shape returned to the frontend (matches `frontend/src/types/time-entry.ts`).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**clock_in** | **datetime** |  | [optional] 
**clock_out** | **datetime** |  | [optional] 
**created_at** | **datetime** |  | 
**var_date** | **date** |  | 
**employee_id** | **UUID** |  | 
**hours** | **str** |  | [optional] 
**notes** | **str** |  | [optional] 
**time_entry_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.time_entry_dto import TimeEntryDto

# TODO update the JSON string below
json = "{}"
# create an instance of TimeEntryDto from a JSON string
time_entry_dto_instance = TimeEntryDto.from_json(json)
# print the JSON string representation of the object
print(TimeEntryDto.to_json())

# convert the object into a dict
time_entry_dto_dict = time_entry_dto_instance.to_dict()
# create an instance of TimeEntryDto from a dict
time_entry_dto_from_dict = TimeEntryDto.from_dict(time_entry_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


