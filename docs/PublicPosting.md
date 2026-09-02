# PublicPosting

Minimal shape for the public careers page (no tenant internals).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **str** |  | [optional] 
**description** | **str** |  | 
**employment_type** | **str** |  | [optional] 
**id** | **UUID** |  | 
**location** | **str** |  | [optional] 
**remote** | **bool** |  | 
**required_skills** | **List[str]** |  | 
**requirements** | **str** |  | [optional] 
**salary_max** | **int** |  | [optional] 
**salary_min** | **int** |  | [optional] 
**title** | **str** |  | 

## Example

```python
from simplebilly_api.models.public_posting import PublicPosting

# TODO update the JSON string below
json = "{}"
# create an instance of PublicPosting from a JSON string
public_posting_instance = PublicPosting.from_json(json)
# print the JSON string representation of the object
print(PublicPosting.to_json())

# convert the object into a dict
public_posting_dict = public_posting_instance.to_dict()
# create an instance of PublicPosting from a dict
public_posting_from_dict = PublicPosting.from_dict(public_posting_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


