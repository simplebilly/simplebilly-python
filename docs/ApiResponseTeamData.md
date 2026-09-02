# ApiResponseTeamData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** |  | 
**description** | **str** |  | [optional] 
**id** | **UUID** |  | 
**name** | **str** |  | 
**parent_team_id** | **UUID** |  | [optional] 
**tenant_id** | **UUID** |  | 
**updated_at** | **datetime** |  | 

## Example

```python
from simplebilly_api.models.api_response_team_data import ApiResponseTeamData

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseTeamData from a JSON string
api_response_team_data_instance = ApiResponseTeamData.from_json(json)
# print the JSON string representation of the object
print(ApiResponseTeamData.to_json())

# convert the object into a dict
api_response_team_data_dict = api_response_team_data_instance.to_dict()
# create an instance of ApiResponseTeamData from a dict
api_response_team_data_from_dict = ApiResponseTeamData.from_dict(api_response_team_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


