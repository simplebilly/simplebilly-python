# PostingCategoryUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_number** | **str** |  | [optional] 
**account_number_skr03** | **str** |  | [optional] 
**account_number_skr04** | **str** |  | [optional] 
**account_number_skr49** | **str** |  | [optional] 
**category_type** | [**PostingCategoryType**](PostingCategoryType.md) |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**default_vat_rate** | **int** |  | [optional] 
**description** | **str** |  | [optional] 
**eks_category** | **str** |  | [optional] 
**eu_vat_line** | **int** |  | [optional] 
**input_vat_percentage** | **str** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**is_system** | **bool** |  | [optional] 
**name** | **str** |  | [optional] 
**skr_version** | **str** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**user_modified_skr03** | **bool** |  | [optional] 
**user_modified_skr04** | **bool** |  | [optional] 

## Example

```python
from simplebilly_api.models.posting_category_update import PostingCategoryUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of PostingCategoryUpdate from a JSON string
posting_category_update_instance = PostingCategoryUpdate.from_json(json)
# print the JSON string representation of the object
print(PostingCategoryUpdate.to_json())

# convert the object into a dict
posting_category_update_dict = posting_category_update_instance.to_dict()
# create an instance of PostingCategoryUpdate from a dict
posting_category_update_from_dict = PostingCategoryUpdate.from_dict(posting_category_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


