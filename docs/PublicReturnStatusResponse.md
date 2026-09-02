# PublicReturnStatusResponse


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
from simplebilly_api.models.public_return_status_response import PublicReturnStatusResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PublicReturnStatusResponse from a JSON string
public_return_status_response_instance = PublicReturnStatusResponse.from_json(json)
# print the JSON string representation of the object
print(PublicReturnStatusResponse.to_json())

# convert the object into a dict
public_return_status_response_dict = public_return_status_response_instance.to_dict()
# create an instance of PublicReturnStatusResponse from a dict
public_return_status_response_from_dict = PublicReturnStatusResponse.from_dict(public_return_status_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


