# BilanzReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**aktiva** | [**List[BilanzItem]**](BilanzItem.md) |  | 
**balanced** | **bool** |  | 
**generated_at** | **str** |  | 
**passiva** | [**List[BilanzItem]**](BilanzItem.md) |  | 
**period** | **str** |  | 
**total_aktiva** | **str** |  | 
**total_passiva** | **str** |  | 

## Example

```python
from simplebilly_api.models.bilanz_report import BilanzReport

# TODO update the JSON string below
json = "{}"
# create an instance of BilanzReport from a JSON string
bilanz_report_instance = BilanzReport.from_json(json)
# print the JSON string representation of the object
print(BilanzReport.to_json())

# convert the object into a dict
bilanz_report_dict = bilanz_report_instance.to_dict()
# create an instance of BilanzReport from a dict
bilanz_report_from_dict = BilanzReport.from_dict(bilanz_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


