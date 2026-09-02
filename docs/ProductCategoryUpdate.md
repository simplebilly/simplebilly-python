# ProductCategoryUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**parent_category_id** | **str** | References the category entity. | [optional] 
**sort_order** | **int** |  | [optional] 

## Example

```python
from simplebilly_api.models.product_category_update import ProductCategoryUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ProductCategoryUpdate from a JSON string
product_category_update_instance = ProductCategoryUpdate.from_json(json)
# print the JSON string representation of the object
print(ProductCategoryUpdate.to_json())

# convert the object into a dict
product_category_update_dict = product_category_update_instance.to_dict()
# create an instance of ProductCategoryUpdate from a dict
product_category_update_from_dict = ProductCategoryUpdate.from_dict(product_category_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


