# TeamCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**name** | **str** |  | 
**parent_team_id** | **UUID** |  | [optional] 

## Example

```python
from simplebilly_api.models.team_create import TeamCreate

# TODO update the JSON string below
json = "{}"
# create an instance of TeamCreate from a JSON string
team_create_instance = TeamCreate.from_json(json)
# print the JSON string representation of the object
print(TeamCreate.to_json())

# convert the object into a dict
team_create_dict = team_create_instance.to_dict()
# create an instance of TeamCreate from a dict
team_create_from_dict = TeamCreate.from_dict(team_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


