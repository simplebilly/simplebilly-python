# JobPosting


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **str** |  | [optional] 
**department** | **str** |  | [optional] 
**description** | **str** | What the job is; markdown/HTML. | 
**employment_type** | [**EmploymentType**](EmploymentType.md) | full_time | part_time | contract | internship | temporary | [optional] 
**location** | **str** |  | [optional] 
**remote** | **bool** |  | 
**required_skills** | **object** | List of required skill names (JSON array of strings). | 
**requirements** | **str** | Structured profile of the required candidate (skills, experience). | [optional] 
**salary_max** | **int** |  | [optional] 
**salary_min** | **int** |  | [optional] 
**status** | [**JobPostingStatus**](JobPostingStatus.md) | draft | published | closed | 
**title** | **str** |  | 

## Example

```python
from simplebilly_api.models.job_posting import JobPosting

# TODO update the JSON string below
json = "{}"
# create an instance of JobPosting from a JSON string
job_posting_instance = JobPosting.from_json(json)
# print the JSON string representation of the object
print(JobPosting.to_json())

# convert the object into a dict
job_posting_dict = job_posting_instance.to_dict()
# create an instance of JobPosting from a dict
job_posting_from_dict = JobPosting.from_dict(job_posting_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


