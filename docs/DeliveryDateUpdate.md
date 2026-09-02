# DeliveryDateUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **str** | References the customer entity. | [optional] 
**fulfilled_date** | **date** | Date actually delivered (set on fulfillment). | [optional] 
**note** | **str** |  | [optional] 
**order_number** | **str** | Sales order number (&#x60;order.order_number&#x60;). | [optional] 
**original_date** | **date** | Original date promised before rescheduling. | [optional] 
**product_id** | **str** | Product line item this date applies to, if per-item. References the product entity. | [optional] 
**promised_date** | **date** | Date promised to the customer. | [optional] 
**status** | [**DeliveryDateStatus**](DeliveryDateStatus.md) | One of: promised | confirmed | rescheduled | fulfilled | late | cancelled | [optional] 

## Example

```python
from simplebilly_api.models.delivery_date_update import DeliveryDateUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of DeliveryDateUpdate from a JSON string
delivery_date_update_instance = DeliveryDateUpdate.from_json(json)
# print the JSON string representation of the object
print(DeliveryDateUpdate.to_json())

# convert the object into a dict
delivery_date_update_dict = delivery_date_update_instance.to_dict()
# create an instance of DeliveryDateUpdate from a dict
delivery_date_update_from_dict = DeliveryDateUpdate.from_dict(delivery_date_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


