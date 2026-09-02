# InventoryCountStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.inventory_count_status_update import InventoryCountStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of InventoryCountStatusUpdate from a JSON string
inventory_count_status_update_instance = InventoryCountStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(InventoryCountStatusUpdate.to_json())

# convert the object into a dict
inventory_count_status_update_dict = inventory_count_status_update_instance.to_dict()
# create an instance of InventoryCountStatusUpdate from a dict
inventory_count_status_update_from_dict = InventoryCountStatusUpdate.from_dict(inventory_count_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


