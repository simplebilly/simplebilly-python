# OffenlegungReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**deadline** | **date** | Fristende (Abschlussstichtag + Frist). | 
**deadline_months** | **int** | Offenlegungsfrist in Monaten (§ 325 Abs. 4 HGB). | 
**items** | [**List[OffenlegungItem]**](OffenlegungItem.md) |  | 
**kapitalmarktorientiert** | **bool** | Annahme über die Kapitalmarktorientierung. | 
**note** | **str** |  | 
**year** | **int** | Berichtsjahr (laufendes Kalenderjahr). | 

## Example

```python
from simplebilly_api.models.offenlegung_report import OffenlegungReport

# TODO update the JSON string below
json = "{}"
# create an instance of OffenlegungReport from a JSON string
offenlegung_report_instance = OffenlegungReport.from_json(json)
# print the JSON string representation of the object
print(OffenlegungReport.to_json())

# convert the object into a dict
offenlegung_report_dict = offenlegung_report_instance.to_dict()
# create an instance of OffenlegungReport from a dict
offenlegung_report_from_dict = OffenlegungReport.from_dict(offenlegung_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


