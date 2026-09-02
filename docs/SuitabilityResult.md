# SuitabilityResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**methods** | [**List[MethodSuitability]**](MethodSuitability.md) |  | 
**recommended_box** | [**BoxFit**](BoxFit.md) |  | [optional] 
**requires_insurance** | **bool** |  | 
**total_value** | **str** |  | 
**total_weight_kg** | **float** |  | 

## Example

```python
from simplebilly_api.models.suitability_result import SuitabilityResult

# TODO update the JSON string below
json = "{}"
# create an instance of SuitabilityResult from a JSON string
suitability_result_instance = SuitabilityResult.from_json(json)
# print the JSON string representation of the object
print(SuitabilityResult.to_json())

# convert the object into a dict
suitability_result_dict = suitability_result_instance.to_dict()
# create an instance of SuitabilityResult from a dict
suitability_result_from_dict = SuitabilityResult.from_dict(suitability_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


