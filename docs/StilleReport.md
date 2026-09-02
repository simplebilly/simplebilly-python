# StilleReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**jahresueberschuss** | **str** |  | 
**partners** | [**List[StillePartnerZeile]**](StillePartnerZeile.md) |  | 
**year** | **int** |  | 

## Example

```python
from simplebilly_api.models.stille_report import StilleReport

# TODO update the JSON string below
json = "{}"
# create an instance of StilleReport from a JSON string
stille_report_instance = StilleReport.from_json(json)
# print the JSON string representation of the object
print(StilleReport.to_json())

# convert the object into a dict
stille_report_dict = stille_report_instance.to_dict()
# create an instance of StilleReport from a dict
stille_report_from_dict = StilleReport.from_dict(stille_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


