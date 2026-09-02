# GdprUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | 
**email** | **str** |  | 
**id** | **UUID** |  | 
**name** | **str** |  | 

## Example

```python
from simplebilly_api.models.gdpr_user import GdprUser

# TODO update the JSON string below
json = "{}"
# create an instance of GdprUser from a JSON string
gdpr_user_instance = GdprUser.from_json(json)
# print the JSON string representation of the object
print(GdprUser.to_json())

# convert the object into a dict
gdpr_user_dict = gdpr_user_instance.to_dict()
# create an instance of GdprUser from a dict
gdpr_user_from_dict = GdprUser.from_dict(gdpr_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


