# AiWorkerConfig


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**auto_reply** | **bool** |  | 
**created_at** | **datetime** |  | 
**id** | **UUID** |  | 
**is_active** | **bool** |  | 
**max_tool_calls** | **int** |  | 
**model** | **str** |  | 
**name** | **str** |  | 
**provider** | **str** |  | 
**system_prompt** | **str** |  | 
**tenant_id** | **UUID** |  | 
**trigger_on** | **List[str]** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.ai_worker_config import AiWorkerConfig

# TODO update the JSON string below
json = "{}"
# create an instance of AiWorkerConfig from a JSON string
ai_worker_config_instance = AiWorkerConfig.from_json(json)
# print the JSON string representation of the object
print(AiWorkerConfig.to_json())

# convert the object into a dict
ai_worker_config_dict = ai_worker_config_instance.to_dict()
# create an instance of AiWorkerConfig from a dict
ai_worker_config_from_dict = AiWorkerConfig.from_dict(ai_worker_config_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


