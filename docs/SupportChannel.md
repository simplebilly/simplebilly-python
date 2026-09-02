# SupportChannel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_type** | [**SupportChannelType**](SupportChannelType.md) |  | 
**config** | **object** |  | 
**created_at** | **datetime** |  | 
**is_active** | **bool** |  | 
**name** | **str** |  | 
**tenant_id** | **UUID** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.support_channel import SupportChannel

# TODO update the JSON string below
json = "{}"
# create an instance of SupportChannel from a JSON string
support_channel_instance = SupportChannel.from_json(json)
# print the JSON string representation of the object
print(SupportChannel.to_json())

# convert the object into a dict
support_channel_dict = support_channel_instance.to_dict()
# create an instance of SupportChannel from a dict
support_channel_from_dict = SupportChannel.from_dict(support_channel_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


