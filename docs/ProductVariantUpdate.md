# ProductVariantUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**barcode** | **str** |  | [optional] 
**image_link** | **str** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**name** | **str** | Human-readable variant label, e.g. \&quot;Red / M\&quot;. | [optional] 
**option_values** | **object** | Option name → value map, e.g. &#x60;{\&quot;Color\&quot;: \&quot;Red\&quot;, \&quot;Size\&quot;: \&quot;M\&quot;}&#x60;. | [optional] 
**price** | **str** | Explicit override price for this variant (takes precedence over parent price + delta). | [optional] 
**price_delta** | **str** | Price adjustment relative to the parent product&#39;s &#x60;default_price&#x60;. | [optional] 
**product_id** | **UUID** | The parent product this variant belongs to. References the product entity. | [optional] 
**sku** | **str** | Variant-specific SKU (must be unique per tenant). | [optional] 
**stock_quantity** | **int** | Variant-level stock (optional — may be tracked on the parent only). | [optional] 

## Example

```python
from simplebilly_api.models.product_variant_update import ProductVariantUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ProductVariantUpdate from a JSON string
product_variant_update_instance = ProductVariantUpdate.from_json(json)
# print the JSON string representation of the object
print(ProductVariantUpdate.to_json())

# convert the object into a dict
product_variant_update_dict = product_variant_update_instance.to_dict()
# create an instance of ProductVariantUpdate from a dict
product_variant_update_from_dict = ProductVariantUpdate.from_dict(product_variant_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


