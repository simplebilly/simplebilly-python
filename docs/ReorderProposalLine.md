# ReorderProposalLine

A single reorder proposal line.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_stock** | **int** |  | 
**max_stock** | **int** |  | [optional] 
**min_stock** | **int** |  | [optional] 
**product_id** | **UUID** |  | 
**product_name** | **str** |  | 
**reorder_quantity** | **int** |  | [optional] 
**sku** | **str** |  | 
**suggested_quantity** | **int** |  | 

## Example

```python
from simplebilly_api.models.reorder_proposal_line import ReorderProposalLine

# TODO update the JSON string below
json = "{}"
# create an instance of ReorderProposalLine from a JSON string
reorder_proposal_line_instance = ReorderProposalLine.from_json(json)
# print the JSON string representation of the object
print(ReorderProposalLine.to_json())

# convert the object into a dict
reorder_proposal_line_dict = reorder_proposal_line_instance.to_dict()
# create an instance of ReorderProposalLine from a dict
reorder_proposal_line_from_dict = ReorderProposalLine.from_dict(reorder_proposal_line_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


