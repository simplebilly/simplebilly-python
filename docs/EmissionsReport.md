# EmissionsReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**by_category** | [**List[CategoryTotal]**](CategoryTotal.md) |  | 
**by_scope** | [**List[ScopeTotal]**](ScopeTotal.md) |  | 
**by_year** | [**List[YearTotal]**](YearTotal.md) |  | 
**data_quality** | [**DataQuality**](DataQuality.md) |  | 
**intensity_per_employee** | **float** |  | [optional] 
**intensity_per_revenue_mio** | **float** | tCO2e per million EUR net revenue. | [optional] 
**net_revenue** | **float** | Sum of paid/sent/partially-paid invoices (EUR net) in the year. | [optional] 
**spend_based_estimate_tco2e** | **float** | Spend-based estimate from bookkeeping payments (EXIOBASE factor). | [optional] 
**targets** | [**List[TargetProgress]**](TargetProgress.md) |  | 
**total_tco2e** | **str** |  | 

## Example

```python
from simplebilly_api.models.emissions_report import EmissionsReport

# TODO update the JSON string below
json = "{}"
# create an instance of EmissionsReport from a JSON string
emissions_report_instance = EmissionsReport.from_json(json)
# print the JSON string representation of the object
print(EmissionsReport.to_json())

# convert the object into a dict
emissions_report_dict = emissions_report_instance.to_dict()
# create an instance of EmissionsReport from a dict
emissions_report_from_dict = EmissionsReport.from_dict(emissions_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


