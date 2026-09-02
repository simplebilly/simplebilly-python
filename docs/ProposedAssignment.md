# ProposedAssignment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount_paid** | **str** |  | 
**confidence** | **float** |  | 
**customer_id** | **str** |  | [optional] 
**invoice_id** | **str** |  | 
**invoice_number** | **str** |  | 
**open_amount** | **str** |  | 
**payment_date** | **str** |  | 
**payment_id** | **UUID** |  | 
**reason** | **str** |  | 
**reference** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.proposed_assignment import ProposedAssignment

# TODO update the JSON string below
json = "{}"
# create an instance of ProposedAssignment from a JSON string
proposed_assignment_instance = ProposedAssignment.from_json(json)
# print the JSON string representation of the object
print(ProposedAssignment.to_json())

# convert the object into a dict
proposed_assignment_dict = proposed_assignment_instance.to_dict()
# create an instance of ProposedAssignment from a dict
proposed_assignment_from_dict = ProposedAssignment.from_dict(proposed_assignment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


