# SyncSummary

Result of a sync/export run — what the app reports back to the admin UI.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error_message** | **str** |  | [optional] 
**items_failed** | **int** |  | [optional] 
**items_synced** | **int** |  | [optional] 

## Example

```python
from simplebilly_api.models.sync_summary import SyncSummary

# TODO update the JSON string below
json = "{}"
# create an instance of SyncSummary from a JSON string
sync_summary_instance = SyncSummary.from_json(json)
# print the JSON string representation of the object
print(SyncSummary.to_json())

# convert the object into a dict
sync_summary_dict = sync_summary_instance.to_dict()
# create an instance of SyncSummary from a dict
sync_summary_from_dict = SyncSummary.from_dict(sync_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


