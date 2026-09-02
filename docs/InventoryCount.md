# InventoryCount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count_date** | **date** |  | 
**count_number** | **str** |  | 
**line_items** | **object** | JSON array of &#x60;{product_id, name, sku, expected_quantity, counted_quantity, bin_location?, batch_number?, variance}&#x60;. | 
**notes** | **str** |  | [optional] 
**status** | [**InventoryCountStatus**](InventoryCountStatus.md) | One of: draft | counting | reviewed | posted | 
**warehouse_id** | **str** | References the warehouse entity. | 

## Example

```python
from simplebilly_api.models.inventory_count import InventoryCount

# TODO update the JSON string below
json = "{}"
# create an instance of InventoryCount from a JSON string
inventory_count_instance = InventoryCount.from_json(json)
# print the JSON string representation of the object
print(InventoryCount.to_json())

# convert the object into a dict
inventory_count_dict = inventory_count_instance.to_dict()
# create an instance of InventoryCount from a dict
inventory_count_from_dict = InventoryCount.from_dict(inventory_count_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


