# GuVItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | **str** |  | 
**amount** | **str** |  | 
**name** | **str** |  | 

## Example

```python
from simplebilly_api.models.gu_v_item import GuVItem

# TODO update the JSON string below
json = "{}"
# create an instance of GuVItem from a JSON string
gu_v_item_instance = GuVItem.from_json(json)
# print the JSON string representation of the object
print(GuVItem.to_json())

# convert the object into a dict
gu_v_item_dict = gu_v_item_instance.to_dict()
# create an instance of GuVItem from a dict
gu_v_item_from_dict = GuVItem.from_dict(gu_v_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


