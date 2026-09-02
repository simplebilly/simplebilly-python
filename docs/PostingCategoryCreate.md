# PostingCategoryCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_number** | **str** |  | [optional] 
**account_number_skr03** | **str** |  | [optional] 
**account_number_skr04** | **str** |  | [optional] 
**account_number_skr49** | **str** |  | [optional] 
**category_type** | [**PostingCategoryType**](PostingCategoryType.md) |  | 
**created_at** | **datetime** |  | 
**default_vat_rate** | **int** |  | 
**description** | **str** |  | [optional] 
**eks_category** | **str** |  | [optional] 
**eu_vat_line** | **int** |  | [optional] 
**input_vat_percentage** | **str** |  | 
**is_active** | **bool** |  | 
**is_system** | **bool** |  | 
**name** | **str** |  | 
**skr_version** | **str** |  | 
**updated_at** | **datetime** |  | [optional] 
**user_modified_skr03** | **bool** |  | 
**user_modified_skr04** | **bool** |  | 

## Example

```python
from simplebilly_api.models.posting_category_create import PostingCategoryCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PostingCategoryCreate from a JSON string
posting_category_create_instance = PostingCategoryCreate.from_json(json)
# print the JSON string representation of the object
print(PostingCategoryCreate.to_json())

# convert the object into a dict
posting_category_create_dict = posting_category_create_instance.to_dict()
# create an instance of PostingCategoryCreate from a dict
posting_category_create_from_dict = PostingCategoryCreate.from_dict(posting_category_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


