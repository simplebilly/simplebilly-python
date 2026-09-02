# PnLItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | **str** |  | 
**account_name** | **str** |  | 
**amount** | **str** |  | 

## Example

```python
from simplebilly_api.models.pn_l_item import PnLItem

# TODO update the JSON string below
json = "{}"
# create an instance of PnLItem from a JSON string
pn_l_item_instance = PnLItem.from_json(json)
# print the JSON string representation of the object
print(PnLItem.to_json())

# convert the object into a dict
pn_l_item_dict = pn_l_item_instance.to_dict()
# create an instance of PnLItem from a dict
pn_l_item_from_dict = PnLItem.from_dict(pn_l_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


