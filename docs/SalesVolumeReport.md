# SalesVolumeReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**grand_total** | **str** |  | 
**items** | [**List[SalesVolumeItem]**](SalesVolumeItem.md) |  | 
**total_count** | **int** |  | 

## Example

```python
from simplebilly_api.models.sales_volume_report import SalesVolumeReport

# TODO update the JSON string below
json = "{}"
# create an instance of SalesVolumeReport from a JSON string
sales_volume_report_instance = SalesVolumeReport.from_json(json)
# print the JSON string representation of the object
print(SalesVolumeReport.to_json())

# convert the object into a dict
sales_volume_report_dict = sales_volume_report_instance.to_dict()
# create an instance of SalesVolumeReport from a dict
sales_volume_report_from_dict = SalesVolumeReport.from_dict(sales_volume_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


