# PriceTierCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_group_id** | **str** | None &#x3D; tier applies to all customers; otherwise a customer group id. | [optional] 
**min_quantity** | **int** | Quantity from which this tier applies (inclusive). | [optional] 
**product_id** | **UUID** | References the product entity. | 
**unit_price** | **str** | Net unit price once &#x60;min_quantity&#x60; is reached. | 

## Example

```python
from simplebilly_api.models.price_tier_create import PriceTierCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PriceTierCreate from a JSON string
price_tier_create_instance = PriceTierCreate.from_json(json)
# print the JSON string representation of the object
print(PriceTierCreate.to_json())

# convert the object into a dict
price_tier_create_dict = price_tier_create_instance.to_dict()
# create an instance of PriceTierCreate from a dict
price_tier_create_from_dict = PriceTierCreate.from_dict(price_tier_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


