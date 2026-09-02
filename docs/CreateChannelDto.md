# CreateChannelDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_type** | **str** |  | 
**config** | **object** |  | 
**name** | **str** |  | 

## Example

```python
from simplebilly_api.models.create_channel_dto import CreateChannelDto

# TODO update the JSON string below
json = "{}"
# create an instance of CreateChannelDto from a JSON string
create_channel_dto_instance = CreateChannelDto.from_json(json)
# print the JSON string representation of the object
print(CreateChannelDto.to_json())

# convert the object into a dict
create_channel_dto_dict = create_channel_dto_instance.to_dict()
# create an instance of CreateChannelDto from a dict
create_channel_dto_from_dict = CreateChannelDto.from_dict(create_channel_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


