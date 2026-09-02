# InstituteCheckItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**exists** | **bool** |  | 
**name** | **str** |  | 
**source** | **str** |  | 

## Example

```python
from simplebilly_api.models.institute_check_item import InstituteCheckItem

# TODO update the JSON string below
json = "{}"
# create an instance of InstituteCheckItem from a JSON string
institute_check_item_instance = InstituteCheckItem.from_json(json)
# print the JSON string representation of the object
print(InstituteCheckItem.to_json())

# convert the object into a dict
institute_check_item_dict = institute_check_item_instance.to_dict()
# create an instance of InstituteCheckItem from a dict
institute_check_item_from_dict = InstituteCheckItem.from_dict(institute_check_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


