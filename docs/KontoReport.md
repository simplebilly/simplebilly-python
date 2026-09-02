# KontoReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**generated_at** | **str** |  | 
**konten** | [**List[KontoItem]**](KontoItem.md) |  | 
**period** | **str** |  | 

## Example

```python
from simplebilly_api.models.konto_report import KontoReport

# TODO update the JSON string below
json = "{}"
# create an instance of KontoReport from a JSON string
konto_report_instance = KontoReport.from_json(json)
# print the JSON string representation of the object
print(KontoReport.to_json())

# convert the object into a dict
konto_report_dict = konto_report_instance.to_dict()
# create an instance of KontoReport from a dict
konto_report_from_dict = KontoReport.from_dict(konto_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


