# ReturnOrderStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.return_order_status_update import ReturnOrderStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ReturnOrderStatusUpdate from a JSON string
return_order_status_update_instance = ReturnOrderStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(ReturnOrderStatusUpdate.to_json())

# convert the object into a dict
return_order_status_update_dict = return_order_status_update_instance.to_dict()
# create an instance of ReturnOrderStatusUpdate from a dict
return_order_status_update_from_dict = ReturnOrderStatusUpdate.from_dict(return_order_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


