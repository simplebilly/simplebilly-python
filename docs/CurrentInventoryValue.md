# CurrentInventoryValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**history** | [**List[InventoryValuePoint]**](InventoryValuePoint.md) |  | 
**product_count** | **int** |  | 
**total_purchase_value** | **str** |  | 
**total_sales_value** | **str** |  | 

## Example

```python
from simplebilly_api.models.current_inventory_value import CurrentInventoryValue

# TODO update the JSON string below
json = "{}"
# create an instance of CurrentInventoryValue from a JSON string
current_inventory_value_instance = CurrentInventoryValue.from_json(json)
# print the JSON string representation of the object
print(CurrentInventoryValue.to_json())

# convert the object into a dict
current_inventory_value_dict = current_inventory_value_instance.to_dict()
# create an instance of CurrentInventoryValue from a dict
current_inventory_value_from_dict = CurrentInventoryValue.from_dict(current_inventory_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


