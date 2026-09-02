# PublicDeliveryAppointmentRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**notes** | **str** |  | [optional] 
**requested_date** | **date** |  | 
**supplier_name** | **str** |  | 
**time_slot** | **str** |  | [optional] 
**warehouse_code** | **str** | Warehouse &#x60;code&#x60; — the supplier does not know the warehouse uuid. | 

## Example

```python
from simplebilly_api.models.public_delivery_appointment_request import PublicDeliveryAppointmentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PublicDeliveryAppointmentRequest from a JSON string
public_delivery_appointment_request_instance = PublicDeliveryAppointmentRequest.from_json(json)
# print the JSON string representation of the object
print(PublicDeliveryAppointmentRequest.to_json())

# convert the object into a dict
public_delivery_appointment_request_dict = public_delivery_appointment_request_instance.to_dict()
# create an instance of PublicDeliveryAppointmentRequest from a dict
public_delivery_appointment_request_from_dict = PublicDeliveryAppointmentRequest.from_dict(public_delivery_appointment_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


