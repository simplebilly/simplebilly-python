# PosTable

A physical table at a restaurant/cafe POS. `current_order_number` links the open order occupying the table; `None` means free.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_order_number** | **str** |  | [optional] 
**name** | **str** |  | 
**status** | [**PosTableStatus**](PosTableStatus.md) |  | [optional] 

## Example

```python
from simplebilly_api.models.pos_table import PosTable

# TODO update the JSON string below
json = "{}"
# create an instance of PosTable from a JSON string
pos_table_instance = PosTable.from_json(json)
# print the JSON string representation of the object
print(PosTable.to_json())

# convert the object into a dict
pos_table_dict = pos_table_instance.to_dict()
# create an instance of PosTable from a dict
pos_table_from_dict = PosTable.from_dict(pos_table_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


