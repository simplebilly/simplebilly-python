# BomCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**components** | **object** | JSON array of &#x60;{product_id, name, quantity, unit, scrap_rate}&#x60;. | [optional] 
**description** | **str** |  | [optional] 
**name** | **str** |  | 
**output_quantity** | **int** | Output quantity per production run (defaults to 1). | [optional] 
**product_id** | **UUID** | The finished product this BOM produces. References the product entity. | 
**status** | [**BomStatus**](BomStatus.md) | One of: draft | active | archived | [optional] 

## Example

```python
from simplebilly_api.models.bom_create import BomCreate

# TODO update the JSON string below
json = "{}"
# create an instance of BomCreate from a JSON string
bom_create_instance = BomCreate.from_json(json)
# print the JSON string representation of the object
print(BomCreate.to_json())

# convert the object into a dict
bom_create_dict = bom_create_instance.to_dict()
# create an instance of BomCreate from a dict
bom_create_from_dict = BomCreate.from_dict(bom_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


