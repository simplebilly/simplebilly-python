# JobTitleGap


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**employee_count** | **int** |  | 
**female_mean_hourly** | **str** |  | 
**job_title** | **str** |  | 
**male_mean_hourly** | **str** |  | 
**mean_gap_pct** | **float** |  | 
**median_gap_pct** | **float** |  | 

## Example

```python
from simplebilly_api.models.job_title_gap import JobTitleGap

# TODO update the JSON string below
json = "{}"
# create an instance of JobTitleGap from a JSON string
job_title_gap_instance = JobTitleGap.from_json(json)
# print the JSON string representation of the object
print(JobTitleGap.to_json())

# convert the object into a dict
job_title_gap_dict = job_title_gap_instance.to_dict()
# create an instance of JobTitleGap from a dict
job_title_gap_from_dict = JobTitleGap.from_dict(job_title_gap_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


