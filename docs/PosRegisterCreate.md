# PosRegisterCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**status** | [**PosRegisterStatus**](PosRegisterStatus.md) |  | [optional] 

## Example

```python
from simplebilly_api.models.pos_register_create import PosRegisterCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PosRegisterCreate from a JSON string
pos_register_create_instance = PosRegisterCreate.from_json(json)
# print the JSON string representation of the object
print(PosRegisterCreate.to_json())

# convert the object into a dict
pos_register_create_dict = pos_register_create_instance.to_dict()
# create an instance of PosRegisterCreate from a dict
pos_register_create_from_dict = PosRegisterCreate.from_dict(pos_register_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


