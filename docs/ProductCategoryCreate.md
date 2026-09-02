# ProductCategoryCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**name** | **str** |  | 
**parent_category_id** | **str** | References the category entity. | [optional] 
**sort_order** | **int** |  | 

## Example

```python
from simplebilly_api.models.product_category_create import ProductCategoryCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ProductCategoryCreate from a JSON string
product_category_create_instance = ProductCategoryCreate.from_json(json)
# print the JSON string representation of the object
print(ProductCategoryCreate.to_json())

# convert the object into a dict
product_category_create_dict = product_category_create_instance.to_dict()
# create an instance of ProductCategoryCreate from a dict
product_category_create_from_dict = ProductCategoryCreate.from_dict(product_category_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


