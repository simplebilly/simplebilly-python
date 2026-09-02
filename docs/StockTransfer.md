# StockTransfer


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**line_items** | **object** | JSON array of &#x60;{product_id, name, quantity, batch_number?}&#x60;. | 
**notes** | **str** |  | [optional] 
**source_warehouse_id** | **str** | References the warehouse entity. | 
**status** | [**StockTransferStatus**](StockTransferStatus.md) | One of: draft | completed | cancelled | 
**target_warehouse_id** | **str** | References the warehouse entity. | 
**transfer_date** | **date** |  | 
**transfer_number** | **str** |  | 

## Example

```python
from simplebilly_api.models.stock_transfer import StockTransfer

# TODO update the JSON string below
json = "{}"
# create an instance of StockTransfer from a JSON string
stock_transfer_instance = StockTransfer.from_json(json)
# print the JSON string representation of the object
print(StockTransfer.to_json())

# convert the object into a dict
stock_transfer_dict = stock_transfer_instance.to_dict()
# create an instance of StockTransfer from a dict
stock_transfer_from_dict = StockTransfer.from_dict(stock_transfer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


