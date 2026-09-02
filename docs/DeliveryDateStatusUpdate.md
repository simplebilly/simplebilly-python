# DeliveryDateStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.delivery_date_status_update import DeliveryDateStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of DeliveryDateStatusUpdate from a JSON string
delivery_date_status_update_instance = DeliveryDateStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(DeliveryDateStatusUpdate.to_json())

# convert the object into a dict
delivery_date_status_update_dict = delivery_date_status_update_instance.to_dict()
# create an instance of DeliveryDateStatusUpdate from a dict
delivery_date_status_update_from_dict = DeliveryDateStatusUpdate.from_dict(delivery_date_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


