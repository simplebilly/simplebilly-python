# EmissionTarget


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**base_value** | **str** |  | 
**base_year** | **int** | tCO2e in the base year (actuals). | 
**description** | **str** | Transition-plan narrative (ESRS E1-1 light), may be empty. | 
**scope** | [**EmissionTargetScope**](EmissionTargetScope.md) | \&quot;total\&quot; | \&quot;1\&quot; | \&quot;2\&quot; | \&quot;3\&quot;. | 
**target_value** | **str** |  | 
**target_year** | **int** | tCO2e target for the target year. | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.emission_target import EmissionTarget

# TODO update the JSON string below
json = "{}"
# create an instance of EmissionTarget from a JSON string
emission_target_instance = EmissionTarget.from_json(json)
# print the JSON string representation of the object
print(EmissionTarget.to_json())

# convert the object into a dict
emission_target_dict = emission_target_instance.to_dict()
# create an instance of EmissionTarget from a dict
emission_target_from_dict = EmissionTarget.from_dict(emission_target_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


