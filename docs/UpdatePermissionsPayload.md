# UpdatePermissionsPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**permissions** | **List[str]** |  | 

## Example

```python
from simplebilly_api.models.update_permissions_payload import UpdatePermissionsPayload

# TODO update the JSON string below
json = "{}"
# create an instance of UpdatePermissionsPayload from a JSON string
update_permissions_payload_instance = UpdatePermissionsPayload.from_json(json)
# print the JSON string representation of the object
print(UpdatePermissionsPayload.to_json())

# convert the object into a dict
update_permissions_payload_dict = update_permissions_payload_instance.to_dict()
# create an instance of UpdatePermissionsPayload from a dict
update_permissions_payload_from_dict = UpdatePermissionsPayload.from_dict(update_permissions_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


