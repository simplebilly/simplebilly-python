# GenerateVariantsRequest

Request body for generating the full variant set from option values.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**options** | **Dict[str, List[str]]** | Option name → list of values, e.g. &#x60;{\&quot;Color\&quot;: [\&quot;Red\&quot;, \&quot;Blue\&quot;], \&quot;Size\&quot;: [\&quot;S\&quot;, \&quot;M\&quot;]}&#x60;. The cartesian product of these lists is generated. | [optional] 
**price_delta** | **str** | Optional per-variant price delta applied to every generated variant. | [optional] 
**product_id** | **UUID** |  | 
**sku_prefix** | **str** | Optional prefix for the generated SKUs (suffix is the option values joined by &#x60;-&#x60;). Falls back to the parent product&#39;s SKU. | [optional] 

## Example

```python
from simplebilly_api.models.generate_variants_request import GenerateVariantsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GenerateVariantsRequest from a JSON string
generate_variants_request_instance = GenerateVariantsRequest.from_json(json)
# print the JSON string representation of the object
print(GenerateVariantsRequest.to_json())

# convert the object into a dict
generate_variants_request_dict = generate_variants_request_instance.to_dict()
# create an instance of GenerateVariantsRequest from a dict
generate_variants_request_from_dict = GenerateVariantsRequest.from_dict(generate_variants_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


