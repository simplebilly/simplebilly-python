# ImportJobStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | **str** | Set only when the job failed. | [optional] 
**job_id** | **str** |  | 
**processed** | **int** |  | 
**progress** | **int** | 0–100 | 
**provider** | **str** | Which competitor the import came from (lexoffice | billbee); the frontend uses it to label the job. Absent for legacy jobs. | [optional] 
**stage** | **str** | queued | fetching | downloading | importing | done | 
**status** | **str** | pending | running | done | failed | 
**total** | **int** |  | 

## Example

```python
from simplebilly_api.models.import_job_status import ImportJobStatus

# TODO update the JSON string below
json = "{}"
# create an instance of ImportJobStatus from a JSON string
import_job_status_instance = ImportJobStatus.from_json(json)
# print the JSON string representation of the object
print(ImportJobStatus.to_json())

# convert the object into a dict
import_job_status_dict = import_job_status_instance.to_dict()
# create an instance of ImportJobStatus from a dict
import_job_status_from_dict = ImportJobStatus.from_dict(import_job_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


