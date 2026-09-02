# ProductionOrderCosting

Actual-costing (Nachkalkulation) report for a production order.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cost_per_unit** | **str** | material_cost_total ÷ quantity. | 
**cost_source** | **str** | \&quot;actual\&quot; when costed from stock-movement consumption, else \&quot;planned\&quot;. | 
**lines** | [**List[CostingLine]**](CostingLine.md) |  | 
**margin_per_unit** | **str** | sale_price − cost_per_unit. | [optional] 
**margin_percent** | **str** | margin_per_unit ÷ cost_per_unit as a percentage. | [optional] 
**material_cost_total** | **str** | Total material cost for the whole order. | 
**order_number** | **str** |  | 
**production_order_id** | **UUID** |  | 
**quantity** | **int** |  | 
**sale_price** | **str** | Finished product&#39;s sale price per unit (used to compute margin). | [optional] 
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.production_order_costing import ProductionOrderCosting

# TODO update the JSON string below
json = "{}"
# create an instance of ProductionOrderCosting from a JSON string
production_order_costing_instance = ProductionOrderCosting.from_json(json)
# print the JSON string representation of the object
print(ProductionOrderCosting.to_json())

# convert the object into a dict
production_order_costing_dict = production_order_costing_instance.to_dict()
# create an instance of ProductionOrderCosting from a dict
production_order_costing_from_dict = ProductionOrderCosting.from_dict(production_order_costing_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


