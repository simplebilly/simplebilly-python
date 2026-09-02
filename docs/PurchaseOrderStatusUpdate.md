# PurchaseOrderStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.purchase_order_status_update import PurchaseOrderStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseOrderStatusUpdate from a JSON string
purchase_order_status_update_instance = PurchaseOrderStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(PurchaseOrderStatusUpdate.to_json())

# convert the object into a dict
purchase_order_status_update_dict = purchase_order_status_update_instance.to_dict()
# create an instance of PurchaseOrderStatusUpdate from a dict
purchase_order_status_update_from_dict = PurchaseOrderStatusUpdate.from_dict(purchase_order_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


