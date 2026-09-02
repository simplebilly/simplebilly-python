# JobApplication


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cv_file** | **str** | Relative path of the stored CV file under the upload dir. | [optional] 
**cv_text** | **str** | Extracted CV text, used for match-scoring. | [optional] 
**email** | **str** |  | [optional] 
**match_reason** | **str** |  | [optional] 
**match_score** | **int** | 0-100 LLM match score against the posting&#39;s required profile. | [optional] 
**name** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**posting_id** | **UUID** | References the job_posting entity. | [optional] 
**source** | **str** | website | email | board | 
**status** | [**ApplicationStatus**](ApplicationStatus.md) | new | reviewing | interview | hired | rejected | 

## Example

```python
from simplebilly_api.models.job_application import JobApplication

# TODO update the JSON string below
json = "{}"
# create an instance of JobApplication from a JSON string
job_application_instance = JobApplication.from_json(json)
# print the JSON string representation of the object
print(JobApplication.to_json())

# convert the object into a dict
job_application_dict = job_application_instance.to_dict()
# create an instance of JobApplication from a dict
job_application_from_dict = JobApplication.from_dict(job_application_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


