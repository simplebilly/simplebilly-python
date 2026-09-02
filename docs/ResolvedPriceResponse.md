# ResolvedPriceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_list_price** | **bool** | True when no tier matched and the product list price was used. | 
**price_tier_id** | **str** | Applied tier, if any matched. | [optional] 
**product_id** | **UUID** |  | 
**quantity** | **int** |  | 
**unit_price** | **str** |  | 

## Example

```python
from simplebilly_api.models.resolved_price_response import ResolvedPriceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ResolvedPriceResponse from a JSON string
resolved_price_response_instance = ResolvedPriceResponse.from_json(json)
# print the JSON string representation of the object
print(ResolvedPriceResponse.to_json())

# convert the object into a dict
resolved_price_response_dict = resolved_price_response_instance.to_dict()
# create an instance of ResolvedPriceResponse from a dict
resolved_price_response_from_dict = ResolvedPriceResponse.from_dict(resolved_price_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


