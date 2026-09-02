# GenerateCountRequest

Body for the cycle-count generator: create a draft count document for a warehouse, optionally restricted to a set of product ids.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**notes** | **str** |  | [optional] 
**product_ids** | **List[UUID]** |  | [optional] 
**warehouse_id** | **str** |  | 

## Example

```python
from simplebilly_api.models.generate_count_request import GenerateCountRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GenerateCountRequest from a JSON string
generate_count_request_instance = GenerateCountRequest.from_json(json)
# print the JSON string representation of the object
print(GenerateCountRequest.to_json())

# convert the object into a dict
generate_count_request_dict = generate_count_request_instance.to_dict()
# create an instance of GenerateCountRequest from a dict
generate_count_request_from_dict = GenerateCountRequest.from_dict(generate_count_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


