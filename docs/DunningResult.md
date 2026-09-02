# DunningResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoices_processed** | **int** |  | 
**message** | **str** |  | 

## Example

```python
from simplebilly_api.models.dunning_result import DunningResult

# TODO update the JSON string below
json = "{}"
# create an instance of DunningResult from a JSON string
dunning_result_instance = DunningResult.from_json(json)
# print the JSON string representation of the object
print(DunningResult.to_json())

# convert the object into a dict
dunning_result_dict = dunning_result_instance.to_dict()
# create an instance of DunningResult from a dict
dunning_result_from_dict = DunningResult.from_dict(dunning_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


