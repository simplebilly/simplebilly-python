# DeliveryAppointmentCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**notes** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**requested_date** | **date** |  | 
**status** | [**DeliveryAppointmentStatus**](DeliveryAppointmentStatus.md) | One of: requested | confirmed | arrived | cancelled | completed | 
**supplier_name** | **str** |  | 
**time_slot** | **str** | e.g. \&quot;08:00-10:00\&quot; | [optional] 
**warehouse_id** | **str** | References the warehouse entity. | 

## Example

```python
from simplebilly_api.models.delivery_appointment_create import DeliveryAppointmentCreate

# TODO update the JSON string below
json = "{}"
# create an instance of DeliveryAppointmentCreate from a JSON string
delivery_appointment_create_instance = DeliveryAppointmentCreate.from_json(json)
# print the JSON string representation of the object
print(DeliveryAppointmentCreate.to_json())

# convert the object into a dict
delivery_appointment_create_dict = delivery_appointment_create_instance.to_dict()
# create an instance of DeliveryAppointmentCreate from a dict
delivery_appointment_create_from_dict = DeliveryAppointmentCreate.from_dict(delivery_appointment_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


