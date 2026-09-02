# ApplicationStatusDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**posting_id** | **UUID** |  | [optional] 
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.application_status_dto import ApplicationStatusDto

# TODO update the JSON string below
json = "{}"
# create an instance of ApplicationStatusDto from a JSON string
application_status_dto_instance = ApplicationStatusDto.from_json(json)
# print the JSON string representation of the object
print(ApplicationStatusDto.to_json())

# convert the object into a dict
application_status_dto_dict = application_status_dto_instance.to_dict()
# create an instance of ApplicationStatusDto from a dict
application_status_dto_from_dict = ApplicationStatusDto.from_dict(application_status_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


