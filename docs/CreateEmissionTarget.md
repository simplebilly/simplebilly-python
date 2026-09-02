# CreateEmissionTarget


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**base_value** | **str** |  | 
**base_year** | **int** |  | 
**description** | **str** |  | 
**scope** | **str** |  | 
**target_value** | **str** |  | 
**target_year** | **int** |  | 

## Example

```python
from simplebilly_api.models.create_emission_target import CreateEmissionTarget

# TODO update the JSON string below
json = "{}"
# create an instance of CreateEmissionTarget from a JSON string
create_emission_target_instance = CreateEmissionTarget.from_json(json)
# print the JSON string representation of the object
print(CreateEmissionTarget.to_json())

# convert the object into a dict
create_emission_target_dict = create_emission_target_instance.to_dict()
# create an instance of CreateEmissionTarget from a dict
create_emission_target_from_dict = CreateEmissionTarget.from_dict(create_emission_target_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


