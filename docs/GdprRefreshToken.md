# GdprRefreshToken


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | 
**expires_at** | **datetime** |  | 
**id** | **UUID** |  | 
**revoked_at** | **datetime** |  | [optional] 
**tenant_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.gdpr_refresh_token import GdprRefreshToken

# TODO update the JSON string below
json = "{}"
# create an instance of GdprRefreshToken from a JSON string
gdpr_refresh_token_instance = GdprRefreshToken.from_json(json)
# print the JSON string representation of the object
print(GdprRefreshToken.to_json())

# convert the object into a dict
gdpr_refresh_token_dict = gdpr_refresh_token_instance.to_dict()
# create an instance of GdprRefreshToken from a dict
gdpr_refresh_token_from_dict = GdprRefreshToken.from_dict(gdpr_refresh_token_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


