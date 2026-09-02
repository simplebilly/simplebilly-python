# RevenueItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** |  | 
**category** | **str** |  | 
**percentage** | **float** |  | 

## Example

```python
from simplebilly_api.models.revenue_item import RevenueItem

# TODO update the JSON string below
json = "{}"
# create an instance of RevenueItem from a JSON string
revenue_item_instance = RevenueItem.from_json(json)
# print the JSON string representation of the object
print(RevenueItem.to_json())

# convert the object into a dict
revenue_item_dict = revenue_item_instance.to_dict()
# create an instance of RevenueItem from a dict
revenue_item_from_dict = RevenueItem.from_dict(revenue_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


