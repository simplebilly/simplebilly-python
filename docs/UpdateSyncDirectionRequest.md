# UpdateSyncDirectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**directions** | **Dict[str, str]** |  | 

## Example

```python
from simplebilly_api.models.update_sync_direction_request import UpdateSyncDirectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateSyncDirectionRequest from a JSON string
update_sync_direction_request_instance = UpdateSyncDirectionRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateSyncDirectionRequest.to_json())

# convert the object into a dict
update_sync_direction_request_dict = update_sync_direction_request_instance.to_dict()
# create an instance of UpdateSyncDirectionRequest from a dict
update_sync_direction_request_from_dict = UpdateSyncDirectionRequest.from_dict(update_sync_direction_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


