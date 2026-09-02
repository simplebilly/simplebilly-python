# ShippingThresholdCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_active** | **bool** |  | [optional] 
**max_sellable** | **int** | Optional ceiling for the deliverable quantity. | [optional] 
**name** | **str** |  | 
**notes** | **str** |  | [optional] 
**product_id** | **UUID** | None &#x3D; applies to all products. References the product entity. | [optional] 
**reserve_stock** | **int** | Buffer of stock that must not be sold. | [optional] 
**warehouse_id** | **str** | None &#x3D; applies to all warehouses. References the warehouse entity. | [optional] 

## Example

```python
from simplebilly_api.models.shipping_threshold_create import ShippingThresholdCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ShippingThresholdCreate from a JSON string
shipping_threshold_create_instance = ShippingThresholdCreate.from_json(json)
# print the JSON string representation of the object
print(ShippingThresholdCreate.to_json())

# convert the object into a dict
shipping_threshold_create_dict = shipping_threshold_create_instance.to_dict()
# create an instance of ShippingThresholdCreate from a dict
shipping_threshold_create_from_dict = ShippingThresholdCreate.from_dict(shipping_threshold_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


