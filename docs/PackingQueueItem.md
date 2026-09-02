# PackingQueueItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **str** |  | 
**customer_id** | **str** |  | 
**delivery_note_printed** | **bool** |  | 
**items** | **object** |  | 
**items_count** | **int** |  | 
**label_printed** | **bool** |  | 
**order_number** | **str** |  | 
**order_status** | **str** |  | 
**shipment_id** | **str** |  | [optional] 
**shipping_address** | **object** |  | [optional] 
**shipping_method** | **str** |  | 
**tracking_number** | **str** |  | [optional] 
**video_recording** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.packing_queue_item import PackingQueueItem

# TODO update the JSON string below
json = "{}"
# create an instance of PackingQueueItem from a JSON string
packing_queue_item_instance = PackingQueueItem.from_json(json)
# print the JSON string representation of the object
print(PackingQueueItem.to_json())

# convert the object into a dict
packing_queue_item_dict = packing_queue_item_instance.to_dict()
# create an instance of PackingQueueItem from a dict
packing_queue_item_from_dict = PackingQueueItem.from_dict(packing_queue_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


