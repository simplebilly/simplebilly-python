# ServiceJobUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **str** | Street + zip + city of the job location. | [optional] 
**customer_email** | **str** | Customer email for email notifications. | [optional] 
**customer_id** | **UUID** | References the customer entity. | [optional] 
**customer_name** | **str** | Denormalized customer name for quick display. | [optional] 
**customer_phone** | **str** | Customer phone for SMS notifications later. | [optional] 
**description** | **str** | What work needs to be done. | [optional] 
**estimated_duration_minutes** | **int** | Estimated time for the job in minutes. | [optional] 
**lat** | **float** | Latitude for map display (OpenStreetMap). | [optional] 
**lng** | **float** | Longitude for map display (OpenStreetMap). | [optional] 
**notes** | **str** |  | [optional] 
**status** | [**ServiceJobStatus**](ServiceJobStatus.md) | Dispatch status: \&quot;pending\&quot;, \&quot;assigned\&quot;, \&quot;en_route\&quot;, \&quot;in_progress\&quot;, \&quot;completed\&quot;, \&quot;cancelled\&quot;. | [optional] 

## Example

```python
from simplebilly_api.models.service_job_update import ServiceJobUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ServiceJobUpdate from a JSON string
service_job_update_instance = ServiceJobUpdate.from_json(json)
# print the JSON string representation of the object
print(ServiceJobUpdate.to_json())

# convert the object into a dict
service_job_update_dict = service_job_update_instance.to_dict()
# create an instance of ServiceJobUpdate from a dict
service_job_update_from_dict = ServiceJobUpdate.from_dict(service_job_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


