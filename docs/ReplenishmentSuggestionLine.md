# ReplenishmentSuggestionLine

A single replenishment suggestion.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_stock** | **int** | Current stock in the target warehouse. | 
**max_stock** | **int** |  | [optional] 
**min_stock** | **int** |  | [optional] 
**product_id** | **UUID** |  | 
**product_name** | **str** |  | 
**sku** | **str** |  | 
**source_available** | **int** | Surplus available in the source warehouse (above its target). | 
**source_warehouse_id** | **str** |  | 
**suggested_quantity** | **int** |  | 
**target_warehouse_id** | **str** |  | 

## Example

```python
from simplebilly_api.models.replenishment_suggestion_line import ReplenishmentSuggestionLine

# TODO update the JSON string below
json = "{}"
# create an instance of ReplenishmentSuggestionLine from a JSON string
replenishment_suggestion_line_instance = ReplenishmentSuggestionLine.from_json(json)
# print the JSON string representation of the object
print(ReplenishmentSuggestionLine.to_json())

# convert the object into a dict
replenishment_suggestion_line_dict = replenishment_suggestion_line_instance.to_dict()
# create an instance of ReplenishmentSuggestionLine from a dict
replenishment_suggestion_line_from_dict = ReplenishmentSuggestionLine.from_dict(replenishment_suggestion_line_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


