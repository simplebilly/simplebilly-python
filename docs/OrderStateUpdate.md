# OrderStateUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**send_state_to_shop** | **bool** |  | [optional] 
**state** | **str** |  | 

## Example

```python
from simplebilly_api.models.order_state_update import OrderStateUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of OrderStateUpdate from a JSON string
order_state_update_instance = OrderStateUpdate.from_json(json)
# print the JSON string representation of the object
print(OrderStateUpdate.to_json())

# convert the object into a dict
order_state_update_dict = order_state_update_instance.to_dict()
# create an instance of OrderStateUpdate from a dict
order_state_update_from_dict = OrderStateUpdate.from_dict(order_state_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


