# Model


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**backup_codes** | **List[str]** |  | 
**created_at** | **datetime** |  | 
**deleted_at** | **datetime** |  | [optional] 
**email** | **str** |  | 
**email_verified** | **bool** |  | 
**id** | **UUID** |  | 
**is_active** | **bool** |  | 
**is_totp_enabled** | **bool** |  | 
**last_login** | **datetime** |  | [optional] 
**name** | **str** |  | 
**oauth_id** | **str** |  | [optional] 
**oauth_provider** | **str** |  | [optional] 
**password_changed_at** | **datetime** | Set on password change; auth/refresh tokens issued before this timestamp are rejected by the auth middleware. | [optional] 
**password_hash** | **str** |  | 
**picture** | **str** |  | [optional] 
**privacy_accepted_at** | **datetime** | When the user accepted the data privacy policy (GDPR consent record). | [optional] 
**totp_secret** | **str** |  | [optional] 
**updated_at** | **datetime** |  | 

## Example

```python
from simplebilly_api.models.model import Model

# TODO update the JSON string below
json = "{}"
# create an instance of Model from a JSON string
model_instance = Model.from_json(json)
# print the JSON string representation of the object
print(Model.to_json())

# convert the object into a dict
model_dict = model_instance.to_dict()
# create an instance of Model from a dict
model_from_dict = Model.from_dict(model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


