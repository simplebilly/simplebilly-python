# SyncLog


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**completed_at** | **datetime** |  | [optional] 
**connection_id** | **str** |  | 
**error_message** | **str** |  | [optional] 
**items_failed** | **int** |  | 
**items_synced** | **int** |  | 
**log_id** | **str** |  | 
**platform** | **str** |  | 
**started_at** | **datetime** |  | 
**status** | **str** |  | 
**sync_type** | **str** |  | 

## Example

```python
from simplebilly_api.models.sync_log import SyncLog

# TODO update the JSON string below
json = "{}"
# create an instance of SyncLog from a JSON string
sync_log_instance = SyncLog.from_json(json)
# print the JSON string representation of the object
print(SyncLog.to_json())

# convert the object into a dict
sync_log_dict = sync_log_instance.to_dict()
# create an instance of SyncLog from a dict
sync_log_from_dict = SyncLog.from_dict(sync_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


