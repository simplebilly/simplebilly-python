# ProductionOrder


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bom_id** | **UUID** | References the BOM entity. | [optional] 
**components** | **object** | JSON snapshot of the BOM components at creation time. | [optional] 
**end_date** | **date** |  | [optional] 
**notes** | **str** |  | [optional] 
**order_number** | **str** |  | 
**product_id** | **UUID** | The finished product to manufacture. References the product entity. | 
**quantity** | **int** | Quantity of finished product to produce. | 
**source_warehouse_id** | **str** | Warehouse components are consumed from. References the warehouse entity. | [optional] 
**start_date** | **date** |  | [optional] 
**status** | [**ProductionOrderStatus**](ProductionOrderStatus.md) | One of: planned | in_production | completed | cancelled | [optional] 
**target_warehouse_id** | **str** | Warehouse the finished product is added to. References the warehouse entity. | [optional] 

## Example

```python
from simplebilly_api.models.production_order import ProductionOrder

# TODO update the JSON string below
json = "{}"
# create an instance of ProductionOrder from a JSON string
production_order_instance = ProductionOrder.from_json(json)
# print the JSON string representation of the object
print(ProductionOrder.to_json())

# convert the object into a dict
production_order_dict = production_order_instance.to_dict()
# create an instance of ProductionOrder from a dict
production_order_from_dict = ProductionOrder.from_dict(production_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


