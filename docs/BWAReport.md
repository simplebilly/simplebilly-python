# BWAReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**expenses** | [**BWAExpenses**](BWAExpenses.md) |  | 
**generated_at** | **str** |  | 
**period** | **str** |  | 
**revenue** | [**BWARevenue**](BWARevenue.md) |  | 
**summary** | [**BWASummary**](BWASummary.md) |  | 

## Example

```python
from simplebilly_api.models.bwa_report import BWAReport

# TODO update the JSON string below
json = "{}"
# create an instance of BWAReport from a JSON string
bwa_report_instance = BWAReport.from_json(json)
# print the JSON string representation of the object
print(BWAReport.to_json())

# convert the object into a dict
bwa_report_dict = bwa_report_instance.to_dict()
# create an instance of BWAReport from a dict
bwa_report_from_dict = BWAReport.from_dict(bwa_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


