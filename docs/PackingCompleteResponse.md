# PackingCompleteResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | 
**new_state** | **str** |  | 
**order_number** | **str** |  | 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.packing_complete_response import PackingCompleteResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PackingCompleteResponse from a JSON string
packing_complete_response_instance = PackingCompleteResponse.from_json(json)
# print the JSON string representation of the object
print(PackingCompleteResponse.to_json())

# convert the object into a dict
packing_complete_response_dict = packing_complete_response_instance.to_dict()
# create an instance of PackingCompleteResponse from a dict
packing_complete_response_from_dict = PackingCompleteResponse.from_dict(packing_complete_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


