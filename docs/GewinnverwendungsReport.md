# GewinnverwendungsReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bilanzgewinn** | **str** | Bilanzgewinn nach Einstellung (§ 174 AktG, Beschluss der HV). | 
**gesetzliche_ruecklage_bestand** | **str** |  | 
**gesetzliche_ruecklage_cap** | **str** | Deckel: 10 % des Grundkapitals (§ 150 Abs. 2 AktG). | 
**gesetzliche_ruecklage_nach** | **str** | Rücklage nach Einstellung. | 
**gesetzliche_ruecklage_soll** | **str** | Vorgeschlagene Einstellung in die gesetzliche Rücklage (§ 150 Abs. 2 AktG). | 
**gezeichnetes_kapital** | **str** |  | 
**jahresueberschuss** | **str** |  | 
**year** | **int** |  | 
**zeilen** | [**List[GewinnverwendungsZeile]**](GewinnverwendungsZeile.md) |  | 

## Example

```python
from simplebilly_api.models.gewinnverwendungs_report import GewinnverwendungsReport

# TODO update the JSON string below
json = "{}"
# create an instance of GewinnverwendungsReport from a JSON string
gewinnverwendungs_report_instance = GewinnverwendungsReport.from_json(json)
# print the JSON string representation of the object
print(GewinnverwendungsReport.to_json())

# convert the object into a dict
gewinnverwendungs_report_dict = gewinnverwendungs_report_instance.to_dict()
# create an instance of GewinnverwendungsReport from a dict
gewinnverwendungs_report_from_dict = GewinnverwendungsReport.from_dict(gewinnverwendungs_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


