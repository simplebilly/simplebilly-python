# PriceTierUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_group_id** | **str** | None &#x3D; tier applies to all customers; otherwise a customer group id. | [optional] 
**min_quantity** | **int** | Quantity from which this tier applies (inclusive). | [optional] 
**product_id** | **UUID** | References the product entity. | [optional] 
**unit_price** | **str** | Net unit price once &#x60;min_quantity&#x60; is reached. | 

## Example

```python
from simplebilly_api.models.price_tier_update import PriceTierUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of PriceTierUpdate from a JSON string
price_tier_update_instance = PriceTierUpdate.from_json(json)
# print the JSON string representation of the object
print(PriceTierUpdate.to_json())

# convert the object into a dict
price_tier_update_dict = price_tier_update_instance.to_dict()
# create an instance of PriceTierUpdate from a dict
price_tier_update_from_dict = PriceTierUpdate.from_dict(price_tier_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


