# CartItemInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product_id** | **UUID** |  | 
**quantity** | **int** |  | 

## Example

```python
from simplebilly_api.models.cart_item_input import CartItemInput

# TODO update the JSON string below
json = "{}"
# create an instance of CartItemInput from a JSON string
cart_item_input_instance = CartItemInput.from_json(json)
# print the JSON string representation of the object
print(CartItemInput.to_json())

# convert the object into a dict
cart_item_input_dict = cart_item_input_instance.to_dict()
# create an instance of CartItemInput from a dict
cart_item_input_from_dict = CartItemInput.from_dict(cart_item_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


