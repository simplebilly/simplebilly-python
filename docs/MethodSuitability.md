# MethodSuitability


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**carrier** | **str** |  | 
**rate** | [**ShippingRate**](ShippingRate.md) |  | [optional] 
**reasons** | **List[str]** |  | 
**service** | **str** |  | 
**suitable** | **bool** |  | 

## Example

```python
from simplebilly_api.models.method_suitability import MethodSuitability

# TODO update the JSON string below
json = "{}"
# create an instance of MethodSuitability from a JSON string
method_suitability_instance = MethodSuitability.from_json(json)
# print the JSON string representation of the object
print(MethodSuitability.to_json())

# convert the object into a dict
method_suitability_dict = method_suitability_instance.to_dict()
# create an instance of MethodSuitability from a dict
method_suitability_from_dict = MethodSuitability.from_dict(method_suitability_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


