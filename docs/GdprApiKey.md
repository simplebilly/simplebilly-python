# GdprApiKey


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | 
**expires_at** | **datetime** |  | [optional] 
**id** | **UUID** |  | 
**key_id** | **UUID** |  | 
**name** | **str** |  | 
**revoked** | **bool** |  | 

## Example

```python
from simplebilly_api.models.gdpr_api_key import GdprApiKey

# TODO update the JSON string below
json = "{}"
# create an instance of GdprApiKey from a JSON string
gdpr_api_key_instance = GdprApiKey.from_json(json)
# print the JSON string representation of the object
print(GdprApiKey.to_json())

# convert the object into a dict
gdpr_api_key_dict = gdpr_api_key_instance.to_dict()
# create an instance of GdprApiKey from a dict
gdpr_api_key_from_dict = GdprApiKey.from_dict(gdpr_api_key_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


