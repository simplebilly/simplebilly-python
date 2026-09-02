# InventoryCountUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count_date** | **date** |  | [optional] 
**count_number** | **str** |  | [optional] 
**line_items** | **object** | JSON array of &#x60;{product_id, name, sku, expected_quantity, counted_quantity, bin_location?, batch_number?, variance}&#x60;. | [optional] 
**notes** | **str** |  | [optional] 
**status** | [**InventoryCountStatus**](InventoryCountStatus.md) | One of: draft | counting | reviewed | posted | [optional] 
**warehouse_id** | **str** | References the warehouse entity. | [optional] 

## Example

```python
from simplebilly_api.models.inventory_count_update import InventoryCountUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of InventoryCountUpdate from a JSON string
inventory_count_update_instance = InventoryCountUpdate.from_json(json)
# print the JSON string representation of the object
print(InventoryCountUpdate.to_json())

# convert the object into a dict
inventory_count_update_dict = inventory_count_update_instance.to_dict()
# create an instance of InventoryCountUpdate from a dict
inventory_count_update_from_dict = InventoryCountUpdate.from_dict(inventory_count_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


