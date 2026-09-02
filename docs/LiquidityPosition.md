# LiquidityPosition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accounts_payable** | **float** |  | 
**accounts_receivable** | **float** |  | 
**cash_and_equivalents** | **float** |  | 
**current_ratio** | **float** |  | 
**quick_ratio** | **float** |  | 
**working_capital** | **float** |  | 

## Example

```python
from simplebilly_api.models.liquidity_position import LiquidityPosition

# TODO update the JSON string below
json = "{}"
# create an instance of LiquidityPosition from a JSON string
liquidity_position_instance = LiquidityPosition.from_json(json)
# print the JSON string representation of the object
print(LiquidityPosition.to_json())

# convert the object into a dict
liquidity_position_dict = liquidity_position_instance.to_dict()
# create an instance of LiquidityPosition from a dict
liquidity_position_from_dict = LiquidityPosition.from_dict(liquidity_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


