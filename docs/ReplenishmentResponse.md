# ReplenishmentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**generated_at** | **datetime** |  | 
**lines** | [**List[ReplenishmentSuggestionLine]**](ReplenishmentSuggestionLine.md) |  | 
**target_warehouse_id** | **str** |  | 
**total_suggested_quantity** | **int** |  | 

## Example

```python
from simplebilly_api.models.replenishment_response import ReplenishmentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ReplenishmentResponse from a JSON string
replenishment_response_instance = ReplenishmentResponse.from_json(json)
# print the JSON string representation of the object
print(ReplenishmentResponse.to_json())

# convert the object into a dict
replenishment_response_dict = replenishment_response_instance.to_dict()
# create an instance of ReplenishmentResponse from a dict
replenishment_response_from_dict = ReplenishmentResponse.from_dict(replenishment_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


