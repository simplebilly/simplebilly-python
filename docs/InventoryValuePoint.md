# InventoryValuePoint


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product_count** | **int** |  | 
**recorded_at** | **datetime** |  | 
**total_purchase_value** | **str** |  | 
**total_sales_value** | **str** |  | 

## Example

```python
from simplebilly_api.models.inventory_value_point import InventoryValuePoint

# TODO update the JSON string below
json = "{}"
# create an instance of InventoryValuePoint from a JSON string
inventory_value_point_instance = InventoryValuePoint.from_json(json)
# print the JSON string representation of the object
print(InventoryValuePoint.to_json())

# convert the object into a dict
inventory_value_point_dict = inventory_value_point_instance.to_dict()
# create an instance of InventoryValuePoint from a dict
inventory_value_point_from_dict = InventoryValuePoint.from_dict(inventory_value_point_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


