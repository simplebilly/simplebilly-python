# BomUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**components** | **object** | JSON array of &#x60;{product_id, name, quantity, unit, scrap_rate}&#x60;. | [optional] 
**description** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**output_quantity** | **int** | Output quantity per production run (defaults to 1). | [optional] 
**product_id** | **UUID** | The finished product this BOM produces. References the product entity. | [optional] 
**status** | [**BomStatus**](BomStatus.md) | One of: draft | active | archived | [optional] 

## Example

```python
from simplebilly_api.models.bom_update import BomUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of BomUpdate from a JSON string
bom_update_instance = BomUpdate.from_json(json)
# print the JSON string representation of the object
print(BomUpdate.to_json())

# convert the object into a dict
bom_update_dict = bom_update_instance.to_dict()
# create an instance of BomUpdate from a dict
bom_update_from_dict = BomUpdate.from_dict(bom_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


