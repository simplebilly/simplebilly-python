# PublicReturnRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 
**items** | [**List[PublicReturnItem]**](PublicReturnItem.md) |  | 
**notes** | **str** |  | [optional] 
**order_number** | **str** |  | 

## Example

```python
from simplebilly_api.models.public_return_request import PublicReturnRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PublicReturnRequest from a JSON string
public_return_request_instance = PublicReturnRequest.from_json(json)
# print the JSON string representation of the object
print(PublicReturnRequest.to_json())

# convert the object into a dict
public_return_request_dict = public_return_request_instance.to_dict()
# create an instance of PublicReturnRequest from a dict
public_return_request_from_dict = PublicReturnRequest.from_dict(public_return_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


