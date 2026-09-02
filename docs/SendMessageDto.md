# SendMessageDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**body** | **str** |  | 
**is_internal** | **bool** |  | [optional] 

## Example

```python
from simplebilly_api.models.send_message_dto import SendMessageDto

# TODO update the JSON string below
json = "{}"
# create an instance of SendMessageDto from a JSON string
send_message_dto_instance = SendMessageDto.from_json(json)
# print the JSON string representation of the object
print(SendMessageDto.to_json())

# convert the object into a dict
send_message_dto_dict = send_message_dto_instance.to_dict()
# create an instance of SendMessageDto from a dict
send_message_dto_from_dict = SendMessageDto.from_dict(send_message_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


