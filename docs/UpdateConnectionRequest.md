# UpdateConnectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_key** | **str** |  | [optional] 
**api_secret** | **str** |  | [optional] 
**config** | **object** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**label** | **str** |  | [optional] 
**shop_domain** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.update_connection_request import UpdateConnectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateConnectionRequest from a JSON string
update_connection_request_instance = UpdateConnectionRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateConnectionRequest.to_json())

# convert the object into a dict
update_connection_request_dict = update_connection_request_instance.to_dict()
# create an instance of UpdateConnectionRequest from a dict
update_connection_request_from_dict = UpdateConnectionRequest.from_dict(update_connection_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


