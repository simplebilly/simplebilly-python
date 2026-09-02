# PayGapReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**by_job_title** | [**List[JobTitleGap]**](JobTitleGap.md) |  | 
**diverse_count** | **int** |  | 
**employee_count** | **int** |  | 
**female_count** | **int** |  | 
**male_count** | **int** |  | 
**mean_gap_pct** | **float** |  | 
**median_gap_pct** | **float** |  | 
**quartiles** | [**List[QuartileBand]**](QuartileBand.md) |  | 

## Example

```python
from simplebilly_api.models.pay_gap_report import PayGapReport

# TODO update the JSON string below
json = "{}"
# create an instance of PayGapReport from a JSON string
pay_gap_report_instance = PayGapReport.from_json(json)
# print the JSON string representation of the object
print(PayGapReport.to_json())

# convert the object into a dict
pay_gap_report_dict = pay_gap_report_instance.to_dict()
# create an instance of PayGapReport from a dict
pay_gap_report_from_dict = PayGapReport.from_dict(pay_gap_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


