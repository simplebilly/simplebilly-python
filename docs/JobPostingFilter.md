# JobPostingFilter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.job_posting_filter import JobPostingFilter

# TODO update the JSON string below
json = "{}"
# create an instance of JobPostingFilter from a JSON string
job_posting_filter_instance = JobPostingFilter.from_json(json)
# print the JSON string representation of the object
print(JobPostingFilter.to_json())

# convert the object into a dict
job_posting_filter_dict = job_posting_filter_instance.to_dict()
# create an instance of JobPostingFilter from a dict
job_posting_filter_from_dict = JobPostingFilter.from_dict(job_posting_filter_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


