# UpdateRolePayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**role** | **str** |  | 
**sync_permissions** | **bool** |  | [optional] 

## Example

```python
from simplebilly_api.models.update_role_payload import UpdateRolePayload

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateRolePayload from a JSON string
update_role_payload_instance = UpdateRolePayload.from_json(json)
# print the JSON string representation of the object
print(UpdateRolePayload.to_json())

# convert the object into a dict
update_role_payload_dict = update_role_payload_instance.to_dict()
# create an instance of UpdateRolePayload from a dict
update_role_payload_from_dict = UpdateRolePayload.from_dict(update_role_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


