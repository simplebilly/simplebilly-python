# PostingCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_number** | **str** |  | [optional] 
**account_number_skr03** | **str** |  | [optional] 
**account_number_skr04** | **str** |  | [optional] 
**account_number_skr49** | **str** |  | [optional] 
**category_id** | **str** |  | 
**default_vat_rate** | **int** |  | 
**description** | **str** |  | [optional] 
**eks_category** | **str** |  | [optional] 
**is_active** | **bool** |  | 
**is_system** | **bool** |  | 
**name** | **str** |  | 
**skr_version** | **str** |  | 
**type** | **str** |  | 

## Example

```python
from simplebilly_api.models.posting_category import PostingCategory

# TODO update the JSON string below
json = "{}"
# create an instance of PostingCategory from a JSON string
posting_category_instance = PostingCategory.from_json(json)
# print the JSON string representation of the object
print(PostingCategory.to_json())

# convert the object into a dict
posting_category_dict = posting_category_instance.to_dict()
# create an instance of PostingCategory from a dict
posting_category_from_dict = PostingCategory.from_dict(posting_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


