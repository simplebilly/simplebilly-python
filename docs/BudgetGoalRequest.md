# BudgetGoalRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**monthly_goal** | **str** | Monthly goal amount (gross). 0 means \&quot;no goal\&quot; (fallback to default). | 
**year** | **int** | Budget year the goal applies to. | 

## Example

```python
from simplebilly_api.models.budget_goal_request import BudgetGoalRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BudgetGoalRequest from a JSON string
budget_goal_request_instance = BudgetGoalRequest.from_json(json)
# print the JSON string representation of the object
print(BudgetGoalRequest.to_json())

# convert the object into a dict
budget_goal_request_dict = budget_goal_request_instance.to_dict()
# create an instance of BudgetGoalRequest from a dict
budget_goal_request_from_dict = BudgetGoalRequest.from_dict(budget_goal_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


