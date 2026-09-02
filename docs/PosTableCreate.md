# PosTableCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_order_number** | **str** |  | [optional] 
**name** | **str** |  | 
**status** | [**PosTableStatus**](PosTableStatus.md) |  | [optional] 

## Example

```python
from simplebilly_api.models.pos_table_create import PosTableCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PosTableCreate from a JSON string
pos_table_create_instance = PosTableCreate.from_json(json)
# print the JSON string representation of the object
print(PosTableCreate.to_json())

# convert the object into a dict
pos_table_create_dict = pos_table_create_instance.to_dict()
# create an instance of PosTableCreate from a dict
pos_table_create_from_dict = PosTableCreate.from_dict(pos_table_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


