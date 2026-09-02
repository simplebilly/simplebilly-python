# ApiResponseVecPlan


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ApiResponseVecPlanDataInner]**](ApiResponseVecPlanDataInner.md) |  | [optional] 
**error** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.api_response_vec_plan import ApiResponseVecPlan

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseVecPlan from a JSON string
api_response_vec_plan_instance = ApiResponseVecPlan.from_json(json)
# print the JSON string representation of the object
print(ApiResponseVecPlan.to_json())

# convert the object into a dict
api_response_vec_plan_dict = api_response_vec_plan_instance.to_dict()
# create an instance of ApiResponseVecPlan from a dict
api_response_vec_plan_from_dict = ApiResponseVecPlan.from_dict(api_response_vec_plan_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


