# StockUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**quantity** | **int** |  | 

## Example

```python
from simplebilly_api.models.stock_update_request import StockUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of StockUpdateRequest from a JSON string
stock_update_request_instance = StockUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(StockUpdateRequest.to_json())

# convert the object into a dict
stock_update_request_dict = stock_update_request_instance.to_dict()
# create an instance of StockUpdateRequest from a dict
stock_update_request_from_dict = StockUpdateRequest.from_dict(stock_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


