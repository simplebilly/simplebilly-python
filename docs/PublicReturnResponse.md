# PublicReturnResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | 
**items** | **object** |  | 
**notes** | **str** |  | [optional] 
**order_number** | **str** |  | [optional] 
**return_number** | **str** |  | 
**return_order_id** | **str** |  | 
**status** | **str** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.public_return_response import PublicReturnResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PublicReturnResponse from a JSON string
public_return_response_instance = PublicReturnResponse.from_json(json)
# print the JSON string representation of the object
print(PublicReturnResponse.to_json())

# convert the object into a dict
public_return_response_dict = public_return_response_instance.to_dict()
# create an instance of PublicReturnResponse from a dict
public_return_response_from_dict = PublicReturnResponse.from_dict(public_return_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


