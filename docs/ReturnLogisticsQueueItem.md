# ReturnLogisticsQueueItem

One open return awaiting warehouse processing (inbound queue).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**age_days** | **int** | Days since creation, oldest first. | 
**created_at** | **datetime** |  | 
**customer_name** | **str** |  | [optional] 
**line_items** | **object** |  | 
**order_number** | **str** |  | [optional] 
**return_number** | **str** |  | 
**return_order_id** | **str** |  | 
**status** | **str** |  | 
**warehouse_id** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.return_logistics_queue_item import ReturnLogisticsQueueItem

# TODO update the JSON string below
json = "{}"
# create an instance of ReturnLogisticsQueueItem from a JSON string
return_logistics_queue_item_instance = ReturnLogisticsQueueItem.from_json(json)
# print the JSON string representation of the object
print(ReturnLogisticsQueueItem.to_json())

# convert the object into a dict
return_logistics_queue_item_dict = return_logistics_queue_item_instance.to_dict()
# create an instance of ReturnLogisticsQueueItem from a dict
return_logistics_queue_item_from_dict = ReturnLogisticsQueueItem.from_dict(return_logistics_queue_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


