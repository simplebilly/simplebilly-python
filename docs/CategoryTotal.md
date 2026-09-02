# CategoryTotal


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category_id** | **str** |  | 
**share_pct** | **float** |  | 
**tco2e** | **str** |  | 

## Example

```python
from simplebilly_api.models.category_total import CategoryTotal

# TODO update the JSON string below
json = "{}"
# create an instance of CategoryTotal from a JSON string
category_total_instance = CategoryTotal.from_json(json)
# print the JSON string representation of the object
print(CategoryTotal.to_json())

# convert the object into a dict
category_total_dict = category_total_instance.to_dict()
# create an instance of CategoryTotal from a dict
category_total_from_dict = CategoryTotal.from_dict(category_total_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


