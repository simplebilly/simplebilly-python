# ProductionOrderStatusUpdate

Status update request.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.production_order_status_update import ProductionOrderStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ProductionOrderStatusUpdate from a JSON string
production_order_status_update_instance = ProductionOrderStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(ProductionOrderStatusUpdate.to_json())

# convert the object into a dict
production_order_status_update_dict = production_order_status_update_instance.to_dict()
# create an instance of ProductionOrderStatusUpdate from a dict
production_order_status_update_from_dict = ProductionOrderStatusUpdate.from_dict(production_order_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


