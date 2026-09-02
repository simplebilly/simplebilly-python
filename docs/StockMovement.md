# StockMovement


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delta** | **int** | Signed movement: positive &#x3D; into stock, negative &#x3D; out of stock. | 
**movement_type** | [**MovementType**](MovementType.md) | One of the &#x60;MOVEMENT_*&#x60; constants. | 
**product_id** | **UUID** | References the product entity. | 
**quantity** | **int** | Absolute quantity moved (always &gt;&#x3D; 0). | 
**reason** | **str** |  | [optional] 
**reference_id** | **str** | Primary-key of the referencing entity. | [optional] 
**reference_type** | [**ReferenceType**](ReferenceType.md) | Entity that caused the movement, e.g. &#x60;goods_receipt&#x60;, &#x60;stock_transfer&#x60;. | [optional] 
**warehouse_id** | **str** | References the warehouse entity. | 

## Example

```python
from simplebilly_api.models.stock_movement import StockMovement

# TODO update the JSON string below
json = "{}"
# create an instance of StockMovement from a JSON string
stock_movement_instance = StockMovement.from_json(json)
# print the JSON string representation of the object
print(StockMovement.to_json())

# convert the object into a dict
stock_movement_dict = stock_movement_instance.to_dict()
# create an instance of StockMovement from a dict
stock_movement_from_dict = StockMovement.from_dict(stock_movement_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


