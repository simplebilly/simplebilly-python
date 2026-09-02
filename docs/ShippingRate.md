# ShippingRate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**breakdown** | **str** |  | [optional] 
**carrier** | **str** |  | 
**cross_border_surcharge** | **str** |  | [optional] 
**destination_country** | **str** | ISO-2 code of destination country. | 
**estimated_days** | **int** |  | [optional] 
**from_api** | **bool** | True when the rate was obtained via an API call rather than calculation. | 
**insured_value** | **str** |  | [optional] 
**island_surcharge** | **str** |  | [optional] 
**origin_country** | **str** | ISO-2 code of origin country. | 
**rate** | **str** |  | 
**service** | **str** |  | 
**volume_discount** | **str** |  | [optional] 
**weight_kg** | **float** |  | 

## Example

```python
from simplebilly_api.models.shipping_rate import ShippingRate

# TODO update the JSON string below
json = "{}"
# create an instance of ShippingRate from a JSON string
shipping_rate_instance = ShippingRate.from_json(json)
# print the JSON string representation of the object
print(ShippingRate.to_json())

# convert the object into a dict
shipping_rate_dict = shipping_rate_instance.to_dict()
# create an instance of ShippingRate from a dict
shipping_rate_from_dict = ShippingRate.from_dict(shipping_rate_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


