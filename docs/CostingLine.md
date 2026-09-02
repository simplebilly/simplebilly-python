# CostingLine

A single costing line: material cost for one BOM component.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**line_cost** | **str** | total_quantity × unit_purchase_price (0 when price unknown). | 
**name** | **str** |  | 
**product_id** | **UUID** |  | 
**quantity_per_unit** | **int** | Component quantity required per finished unit. | 
**sku** | **str** |  | 
**total_quantity** | **int** | Total component quantity consumed by this order. | 
**unit_purchase_price** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.costing_line import CostingLine

# TODO update the JSON string below
json = "{}"
# create an instance of CostingLine from a JSON string
costing_line_instance = CostingLine.from_json(json)
# print the JSON string representation of the object
print(CostingLine.to_json())

# convert the object into a dict
costing_line_dict = costing_line_instance.to_dict()
# create an instance of CostingLine from a dict
costing_line_from_dict = CostingLine.from_dict(costing_line_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


