# OffenlegungItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**exists** | **bool** | Ob die zugrunde liegenden Daten im System vorhanden sind. | 
**name** | **str** | Bezeichnung des Offenlegungsbestandteils (§ 325 Abs. 1 HGB). | 
**source** | **str** | Woher der Bestandteil stammt bzw. fehlt. | 

## Example

```python
from simplebilly_api.models.offenlegung_item import OffenlegungItem

# TODO update the JSON string below
json = "{}"
# create an instance of OffenlegungItem from a JSON string
offenlegung_item_instance = OffenlegungItem.from_json(json)
# print the JSON string representation of the object
print(OffenlegungItem.to_json())

# convert the object into a dict
offenlegung_item_dict = offenlegung_item_instance.to_dict()
# create an instance of OffenlegungItem from a dict
offenlegung_item_from_dict = OffenlegungItem.from_dict(offenlegung_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


