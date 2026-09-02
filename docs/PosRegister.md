# PosRegister

A point-of-sale register (Kasse). Registers are the billable unit of the POS feature: each active register costs a monthly fee per tenant, billed through Paddle. `status`: `active` | `disabled`.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**status** | [**PosRegisterStatus**](PosRegisterStatus.md) |  | [optional] 

## Example

```python
from simplebilly_api.models.pos_register import PosRegister

# TODO update the JSON string below
json = "{}"
# create an instance of PosRegister from a JSON string
pos_register_instance = PosRegister.from_json(json)
# print the JSON string representation of the object
print(PosRegister.to_json())

# convert the object into a dict
pos_register_dict = pos_register_instance.to_dict()
# create an instance of PosRegister from a dict
pos_register_from_dict = PosRegister.from_dict(pos_register_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


