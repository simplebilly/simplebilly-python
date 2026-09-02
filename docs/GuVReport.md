# GuVReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**expenses** | [**List[GuVItem]**](GuVItem.md) |  | 
**generated_at** | **str** |  | 
**net_income** | **str** |  | 
**period** | **str** |  | 
**revenue** | [**List[GuVItem]**](GuVItem.md) |  | 
**total_expenses** | **str** |  | 
**total_revenue** | **str** |  | 

## Example

```python
from simplebilly_api.models.gu_v_report import GuVReport

# TODO update the JSON string below
json = "{}"
# create an instance of GuVReport from a JSON string
gu_v_report_instance = GuVReport.from_json(json)
# print the JSON string representation of the object
print(GuVReport.to_json())

# convert the object into a dict
gu_v_report_dict = gu_v_report_instance.to_dict()
# create an instance of GuVReport from a dict
gu_v_report_from_dict = GuVReport.from_dict(gu_v_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


