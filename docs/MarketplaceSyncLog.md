# MarketplaceSyncLog


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**completed_at** | **datetime** |  | [optional] 
**connection_id** | **str** | References the marketplace connection entity. | 
**error_message** | **str** |  | [optional] 
**items_failed** | **int** |  | 
**items_synced** | **int** |  | 
**platform** | **str** |  | 
**started_at** | **datetime** |  | 
**status** | [**SyncLogStatus**](SyncLogStatus.md) |  | 
**sync_type** | [**SyncType**](SyncType.md) |  | 

## Example

```python
from simplebilly_api.models.marketplace_sync_log import MarketplaceSyncLog

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceSyncLog from a JSON string
marketplace_sync_log_instance = MarketplaceSyncLog.from_json(json)
# print the JSON string representation of the object
print(MarketplaceSyncLog.to_json())

# convert the object into a dict
marketplace_sync_log_dict = marketplace_sync_log_instance.to_dict()
# create an instance of MarketplaceSyncLog from a dict
marketplace_sync_log_from_dict = MarketplaceSyncLog.from_dict(marketplace_sync_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


