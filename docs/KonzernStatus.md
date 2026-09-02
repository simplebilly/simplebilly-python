# KonzernStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**groessenbefreit** | **bool** |  | 
**kapitalmarktorientiert** | **bool** |  | 
**konzernabschlusspflicht** | **bool** |  | 
**missing_group_figures** | **bool** | Keine group_figures-Zeile für das Jahr vorhanden → keine Größenbefreiung. | 
**mutterunternehmen** | **bool** | Mutterunternehmen: mindestens eine beherrschte Beteiligung (§ 290 Abs. 1 HGB). | 
**parent_name** | **str** | Mutterunternehmen für die Zwischenholding-Befreiung (§ 291 HGB). | [optional] 
**parent_situs** | **str** |  | [optional] 
**participations** | [**List[KonzernBeteiligung]**](KonzernBeteiligung.md) |  | 
**thresholds** | [**KonzernThresholds**](KonzernThresholds.md) |  | 
**year** | **int** |  | 
**zwischenholding_befreit** | **bool** |  | 
**zwischenholding_hinweis** | **str** | Hinweis zu den § 291-Voraussetzungen (EU/EWR-Sitz, geprüfter Konzernabschluss). | [optional] 

## Example

```python
from simplebilly_api.models.konzern_status import KonzernStatus

# TODO update the JSON string below
json = "{}"
# create an instance of KonzernStatus from a JSON string
konzern_status_instance = KonzernStatus.from_json(json)
# print the JSON string representation of the object
print(KonzernStatus.to_json())

# convert the object into a dict
konzern_status_dict = konzern_status_instance.to_dict()
# create an instance of KonzernStatus from a dict
konzern_status_from_dict = KonzernStatus.from_dict(konzern_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


