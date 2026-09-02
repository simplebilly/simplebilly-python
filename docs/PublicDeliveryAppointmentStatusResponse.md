# PublicDeliveryAppointmentStatusResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appointment_id** | **str** |  | 
**requested_date** | **date** |  | 
**status** | **str** |  | 
**time_slot** | **str** |  | [optional] 
**warehouse_name** | **str** |  | 

## Example

```python
from simplebilly_api.models.public_delivery_appointment_status_response import PublicDeliveryAppointmentStatusResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PublicDeliveryAppointmentStatusResponse from a JSON string
public_delivery_appointment_status_response_instance = PublicDeliveryAppointmentStatusResponse.from_json(json)
# print the JSON string representation of the object
print(PublicDeliveryAppointmentStatusResponse.to_json())

# convert the object into a dict
public_delivery_appointment_status_response_dict = public_delivery_appointment_status_response_instance.to_dict()
# create an instance of PublicDeliveryAppointmentStatusResponse from a dict
public_delivery_appointment_status_response_from_dict = PublicDeliveryAppointmentStatusResponse.from_dict(public_delivery_appointment_status_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


