# LaborCostRow


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cost** | **str** |  | 
**employee_id** | **UUID** |  | [optional] 
**group_key** | **str** |  | 
**hours** | **str** |  | 
**name** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.labor_cost_row import LaborCostRow

# TODO update the JSON string below
json = "{}"
# create an instance of LaborCostRow from a JSON string
labor_cost_row_instance = LaborCostRow.from_json(json)
# print the JSON string representation of the object
print(LaborCostRow.to_json())

# convert the object into a dict
labor_cost_row_dict = labor_cost_row_instance.to_dict()
# create an instance of LaborCostRow from a dict
labor_cost_row_from_dict = LaborCostRow.from_dict(labor_cost_row_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


