# EmissionFactorResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category_id** | **str** |  | 
**kg_co2e_per_unit** | **float** |  | 
**name_de** | **str** |  | 
**source** | **str** |  | 
**unit** | **str** |  | 
**version** | **str** |  | 

## Example

```python
from simplebilly_api.models.emission_factor_response import EmissionFactorResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EmissionFactorResponse from a JSON string
emission_factor_response_instance = EmissionFactorResponse.from_json(json)
# print the JSON string representation of the object
print(EmissionFactorResponse.to_json())

# convert the object into a dict
emission_factor_response_dict = emission_factor_response_instance.to_dict()
# create an instance of EmissionFactorResponse from a dict
emission_factor_response_from_dict = EmissionFactorResponse.from_dict(emission_factor_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


