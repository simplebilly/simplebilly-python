# UpdateChannelDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config** | **object** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.update_channel_dto import UpdateChannelDto

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateChannelDto from a JSON string
update_channel_dto_instance = UpdateChannelDto.from_json(json)
# print the JSON string representation of the object
print(UpdateChannelDto.to_json())

# convert the object into a dict
update_channel_dto_dict = update_channel_dto_instance.to_dict()
# create an instance of UpdateChannelDto from a dict
update_channel_dto_from_dict = UpdateChannelDto.from_dict(update_channel_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


