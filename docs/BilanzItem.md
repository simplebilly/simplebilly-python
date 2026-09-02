# BilanzItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** |  | 
**konto** | **str** |  | 
**name** | **str** |  | 

## Example

```python
from simplebilly_api.models.bilanz_item import BilanzItem

# TODO update the JSON string below
json = "{}"
# create an instance of BilanzItem from a JSON string
bilanz_item_instance = BilanzItem.from_json(json)
# print the JSON string representation of the object
print(BilanzItem.to_json())

# convert the object into a dict
bilanz_item_dict = bilanz_item_instance.to_dict()
# create an instance of BilanzItem from a dict
bilanz_item_from_dict = BilanzItem.from_dict(bilanz_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


