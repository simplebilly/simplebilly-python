# Job


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**attempts** | **int** |  | [optional] 
**job_type** | **str** | Discriminator the worker dispatches on (e.g. \&quot;webhook.deliver\&quot;). | 
**max_attempts** | **int** |  | 
**payload** | **object** |  | [optional] 
**run_at** | **datetime** | Earliest execution time; None &#x3D; run now. | [optional] 
**status** | [**JobStatus**](JobStatus.md) | pending | running | done | failed | 

## Example

```python
from simplebilly_api.models.job import Job

# TODO update the JSON string below
json = "{}"
# create an instance of Job from a JSON string
job_instance = Job.from_json(json)
# print the JSON string representation of the object
print(Job.to_json())

# convert the object into a dict
job_dict = job_instance.to_dict()
# create an instance of Job from a dict
job_from_dict = Job.from_dict(job_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


