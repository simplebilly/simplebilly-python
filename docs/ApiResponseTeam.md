# ApiResponseTeam


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ApiResponseTeamData**](ApiResponseTeamData.md) |  | [optional] 
**error** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.api_response_team import ApiResponseTeam

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseTeam from a JSON string
api_response_team_instance = ApiResponseTeam.from_json(json)
# print the JSON string representation of the object
print(ApiResponseTeam.to_json())

# convert the object into a dict
api_response_team_dict = api_response_team_instance.to_dict()
# create an instance of ApiResponseTeam from a dict
api_response_team_from_dict = ApiResponseTeam.from_dict(api_response_team_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


