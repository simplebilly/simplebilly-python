# KontoItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**anfangsbestand** | **str** |  | 
**haben_umsatz** | **str** |  | 
**konto** | **str** |  | 
**name** | **str** |  | 
**saldo** | **str** |  | 
**soll_umsatz** | **str** |  | 

## Example

```python
from simplebilly_api.models.konto_item import KontoItem

# TODO update the JSON string below
json = "{}"
# create an instance of KontoItem from a JSON string
konto_item_instance = KontoItem.from_json(json)
# print the JSON string representation of the object
print(KontoItem.to_json())

# convert the object into a dict
konto_item_dict = konto_item_instance.to_dict()
# create an instance of KontoItem from a dict
konto_item_from_dict = KontoItem.from_dict(konto_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


