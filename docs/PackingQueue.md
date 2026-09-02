# PackingQueue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[PackingQueueItem]**](PackingQueueItem.md) |  | 
**page** | **int** |  | 
**page_size** | **int** |  | 
**total_count** | **int** |  | 

## Example

```python
from simplebilly_api.models.packing_queue import PackingQueue

# TODO update the JSON string below
json = "{}"
# create an instance of PackingQueue from a JSON string
packing_queue_instance = PackingQueue.from_json(json)
# print the JSON string representation of the object
print(PackingQueue.to_json())

# convert the object into a dict
packing_queue_dict = packing_queue_instance.to_dict()
# create an instance of PackingQueue from a dict
packing_queue_from_dict = PackingQueue.from_dict(packing_queue_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


