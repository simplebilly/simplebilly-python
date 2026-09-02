# AppointmentStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.appointment_status_update import AppointmentStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AppointmentStatusUpdate from a JSON string
appointment_status_update_instance = AppointmentStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(AppointmentStatusUpdate.to_json())

# convert the object into a dict
appointment_status_update_dict = appointment_status_update_instance.to_dict()
# create an instance of AppointmentStatusUpdate from a dict
appointment_status_update_from_dict = AppointmentStatusUpdate.from_dict(appointment_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


