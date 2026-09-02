# WarehouseStock


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**batch_number** | **str** | Batch/lot number (Chargennummer) — &#x60;None&#x60; for non-batched goods. | [optional] 
**bin_location** | **str** |  | [optional] 
**expiry_date** | **date** | Expiry date for batch-tracked goods. | [optional] 
**product_id** | **UUID** |  | 
**quantity** | **int** |  | 
**serial_numbers** | **object** | JSON array of serial numbers (Seriennummern) in this stock row. | [optional] 
**warehouse_id** | **str** |  | 

## Example

```python
from simplebilly_api.models.warehouse_stock import WarehouseStock

# TODO update the JSON string below
json = "{}"
# create an instance of WarehouseStock from a JSON string
warehouse_stock_instance = WarehouseStock.from_json(json)
# print the JSON string representation of the object
print(WarehouseStock.to_json())

# convert the object into a dict
warehouse_stock_dict = warehouse_stock_instance.to_dict()
# create an instance of WarehouseStock from a dict
warehouse_stock_from_dict = WarehouseStock.from_dict(warehouse_stock_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


