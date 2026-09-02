# ApiResponseVecTeam


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ApiResponseTeamData]**](ApiResponseTeamData.md) |  | [optional] 
**error** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.api_response_vec_team import ApiResponseVecTeam

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseVecTeam from a JSON string
api_response_vec_team_instance = ApiResponseVecTeam.from_json(json)
# print the JSON string representation of the object
print(ApiResponseVecTeam.to_json())

# convert the object into a dict
api_response_vec_team_dict = api_response_vec_team_instance.to_dict()
# create an instance of ApiResponseVecTeam from a dict
api_response_vec_team_from_dict = ApiResponseVecTeam.from_dict(api_response_vec_team_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


