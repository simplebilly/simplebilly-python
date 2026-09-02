# ProductStock


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**product_id** | **UUID** |  | 
**sku** | **str** |  | 
**stock_quantity** | **int** |  | [optional] 

## Example

```python
from simplebilly_api.models.product_stock import ProductStock

# TODO update the JSON string below
json = "{}"
# create an instance of ProductStock from a JSON string
product_stock_instance = ProductStock.from_json(json)
# print the JSON string representation of the object
print(ProductStock.to_json())

# convert the object into a dict
product_stock_dict = product_stock_instance.to_dict()
# create an instance of ProductStock from a dict
product_stock_from_dict = ProductStock.from_dict(product_stock_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


