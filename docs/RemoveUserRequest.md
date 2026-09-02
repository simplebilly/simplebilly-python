# RemoveUserRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 

## Example

```python
from simplebilly_api.models.remove_user_request import RemoveUserRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RemoveUserRequest from a JSON string
remove_user_request_instance = RemoveUserRequest.from_json(json)
# print the JSON string representation of the object
print(RemoveUserRequest.to_json())

# convert the object into a dict
remove_user_request_dict = remove_user_request_instance.to_dict()
# create an instance of RemoveUserRequest from a dict
remove_user_request_from_dict = RemoveUserRequest.from_dict(remove_user_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


