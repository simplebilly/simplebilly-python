# GroupFigureCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bilanzsumme** | **str** | Bilanzsumme in EUR (§ 293 Abs. 1 Nr. 1 HGB). | [optional] 
**exemption_claimed** | **bool** | § 291-Befreiung in Anspruch genommen. | [optional] 
**mitarbeiter** | **int** | Durchschnittliche Arbeitnehmerzahl (§ 293 Abs. 1 Nr. 3 HGB). | [optional] 
**netto_umsatz** | **str** | Netto-Umsatzerlöse in EUR (§ 293 Abs. 1 Nr. 2 HGB). | [optional] 
**parent_name** | **str** | Name des Mutterunternehmens (§ 291 HGB, Zwischenholding). | [optional] 
**parent_situs** | **str** | Sitz des Mutterunternehmens, z. B. \&quot;EU/EWR\&quot; (§ 291 HGB). | [optional] 

## Example

```python
from simplebilly_api.models.group_figure_create import GroupFigureCreate

# TODO update the JSON string below
json = "{}"
# create an instance of GroupFigureCreate from a JSON string
group_figure_create_instance = GroupFigureCreate.from_json(json)
# print the JSON string representation of the object
print(GroupFigureCreate.to_json())

# convert the object into a dict
group_figure_create_dict = group_figure_create_instance.to_dict()
# create an instance of GroupFigureCreate from a dict
group_figure_create_from_dict = GroupFigureCreate.from_dict(group_figure_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


