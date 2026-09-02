# StockTransferStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.stock_transfer_status_update import StockTransferStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of StockTransferStatusUpdate from a JSON string
stock_transfer_status_update_instance = StockTransferStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(StockTransferStatusUpdate.to_json())

# convert the object into a dict
stock_transfer_status_update_dict = stock_transfer_status_update_instance.to_dict()
# create an instance of StockTransferStatusUpdate from a dict
stock_transfer_status_update_from_dict = StockTransferStatusUpdate.from_dict(stock_transfer_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


