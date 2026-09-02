# ProductAttribute


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_filterable** | **bool** | Whether this attribute participates in the shop&#39;s faceted filters. | [optional] 
**name** | **str** | Attribute name, e.g. &#x60;Material&#x60;, &#x60;Farbe&#x60;, &#x60;Gewicht&#x60;. | 
**position** | **int** | Ordering position within the product&#39;s attribute list. | [optional] 
**product_id** | **UUID** | The product this attribute belongs to. References the product entity. | 
**unit** | **str** | Optional unit of measure for numeric attributes, e.g. &#x60;g&#x60;, &#x60;cm&#x60;. | [optional] 
**value** | **str** | Attribute value, e.g. &#x60;Baumwolle&#x60;, &#x60;Rot&#x60;, &#x60;180g&#x60;. | 

## Example

```python
from simplebilly_api.models.product_attribute import ProductAttribute

# TODO update the JSON string below
json = "{}"
# create an instance of ProductAttribute from a JSON string
product_attribute_instance = ProductAttribute.from_json(json)
# print the JSON string representation of the object
print(ProductAttribute.to_json())

# convert the object into a dict
product_attribute_dict = product_attribute_instance.to_dict()
# create an instance of ProductAttribute from a dict
product_attribute_from_dict = ProductAttribute.from_dict(product_attribute_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


