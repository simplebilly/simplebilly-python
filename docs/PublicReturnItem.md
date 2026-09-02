# PublicReturnItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**product_id** | **str** |  | 
**quantity** | **int** |  | 
**reason** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.public_return_item import PublicReturnItem

# TODO update the JSON string below
json = "{}"
# create an instance of PublicReturnItem from a JSON string
public_return_item_instance = PublicReturnItem.from_json(json)
# print the JSON string representation of the object
print(PublicReturnItem.to_json())

# convert the object into a dict
public_return_item_dict = public_return_item_instance.to_dict()
# create an instance of PublicReturnItem from a dict
public_return_item_from_dict = PublicReturnItem.from_dict(public_return_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


