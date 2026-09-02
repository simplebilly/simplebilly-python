# GezReport

Berechnungsergebnis des Rundfunkbeitrags für ein Unternehmen.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**beitragsfreie_kfz** | **int** |  | 
**beitragspflichtige_kfz** | **int** |  | 
**betriebsstaetten** | [**List[BetriebsstaettenDetail]**](BetriebsstaettenDetail.md) |  | 
**hinweis** | **str** |  | 
**hotelzimmer_beitrag** | **str** |  | 
**jaehrlicher_beitrag** | **str** |  | 
**jahr** | **int** |  | 
**kfz_beitrag** | **str** |  | 
**monatlicher_beitrag** | **str** |  | 
**vierteljaehrlicher_beitrag** | **str** |  | 

## Example

```python
from simplebilly_api.models.gez_report import GezReport

# TODO update the JSON string below
json = "{}"
# create an instance of GezReport from a JSON string
gez_report_instance = GezReport.from_json(json)
# print the JSON string representation of the object
print(GezReport.to_json())

# convert the object into a dict
gez_report_dict = gez_report_instance.to_dict()
# create an instance of GezReport from a dict
gez_report_from_dict = GezReport.from_dict(gez_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


