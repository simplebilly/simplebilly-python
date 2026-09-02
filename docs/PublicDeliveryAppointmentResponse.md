# PublicDeliveryAppointmentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**appointment_id** | **str** |  | 
**confirmation_hint** | **str** | Carries the status-check token (email is out of scope for now). | 
**message** | **str** |  | 
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.public_delivery_appointment_response import PublicDeliveryAppointmentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PublicDeliveryAppointmentResponse from a JSON string
public_delivery_appointment_response_instance = PublicDeliveryAppointmentResponse.from_json(json)
# print the JSON string representation of the object
print(PublicDeliveryAppointmentResponse.to_json())

# convert the object into a dict
public_delivery_appointment_response_dict = public_delivery_appointment_response_instance.to_dict()
# create an instance of PublicDeliveryAppointmentResponse from a dict
public_delivery_appointment_response_from_dict = PublicDeliveryAppointmentResponse.from_dict(public_delivery_appointment_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


