# DeliveryDate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **str** | References the customer entity. | [optional] 
**fulfilled_date** | **date** | Date actually delivered (set on fulfillment). | [optional] 
**note** | **str** |  | [optional] 
**order_number** | **str** | Sales order number (&#x60;order.order_number&#x60;). | 
**original_date** | **date** | Original date promised before rescheduling. | [optional] 
**product_id** | **str** | Product line item this date applies to, if per-item. References the product entity. | [optional] 
**promised_date** | **date** | Date promised to the customer. | 
**status** | [**DeliveryDateStatus**](DeliveryDateStatus.md) | One of: promised | confirmed | rescheduled | fulfilled | late | cancelled | 

## Example

```python
from simplebilly_api.models.delivery_date import DeliveryDate

# TODO update the JSON string below
json = "{}"
# create an instance of DeliveryDate from a JSON string
delivery_date_instance = DeliveryDate.from_json(json)
# print the JSON string representation of the object
print(DeliveryDate.to_json())

# convert the object into a dict
delivery_date_dict = delivery_date_instance.to_dict()
# create an instance of DeliveryDate from a dict
delivery_date_from_dict = DeliveryDate.from_dict(delivery_date_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


