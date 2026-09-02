# StockAdjustment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**batch_number** | **str** |  | [optional] 
**bin_location** | **str** |  | [optional] 
**expiry_date** | **date** |  | [optional] 
**product_id** | **UUID** |  | [optional] 
**quantity** | **int** |  | 
**serial_numbers** | **List[str]** |  | [optional] 

## Example

```python
from simplebilly_api.models.stock_adjustment import StockAdjustment

# TODO update the JSON string below
json = "{}"
# create an instance of StockAdjustment from a JSON string
stock_adjustment_instance = StockAdjustment.from_json(json)
# print the JSON string representation of the object
print(StockAdjustment.to_json())

# convert the object into a dict
stock_adjustment_dict = stock_adjustment_instance.to_dict()
# create an instance of StockAdjustment from a dict
stock_adjustment_from_dict = StockAdjustment.from_dict(stock_adjustment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


