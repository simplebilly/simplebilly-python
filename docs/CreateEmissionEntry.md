# CreateEmissionEntry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activity_value** | **str** |  | 
**category_id** | **str** |  | 
**description** | **str** |  | 
**method** | **str** |  | 
**scope** | **str** |  | 
**unit** | **str** |  | 
**year** | **int** |  | 

## Example

```python
from simplebilly_api.models.create_emission_entry import CreateEmissionEntry

# TODO update the JSON string below
json = "{}"
# create an instance of CreateEmissionEntry from a JSON string
create_emission_entry_instance = CreateEmissionEntry.from_json(json)
# print the JSON string representation of the object
print(CreateEmissionEntry.to_json())

# convert the object into a dict
create_emission_entry_dict = create_emission_entry_instance.to_dict()
# create an instance of CreateEmissionEntry from a dict
create_emission_entry_from_dict = CreateEmissionEntry.from_dict(create_emission_entry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


