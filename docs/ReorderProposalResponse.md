# ReorderProposalResponse

The response envelope for a reorder proposal run.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**generated_at** | **datetime** |  | 
**lines** | [**List[ReorderProposalLine]**](ReorderProposalLine.md) |  | 
**total_suggested_quantity** | **int** |  | 

## Example

```python
from simplebilly_api.models.reorder_proposal_response import ReorderProposalResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ReorderProposalResponse from a JSON string
reorder_proposal_response_instance = ReorderProposalResponse.from_json(json)
# print the JSON string representation of the object
print(ReorderProposalResponse.to_json())

# convert the object into a dict
reorder_proposal_response_dict = reorder_proposal_response_instance.to_dict()
# create an instance of ReorderProposalResponse from a dict
reorder_proposal_response_from_dict = ReorderProposalResponse.from_dict(reorder_proposal_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


