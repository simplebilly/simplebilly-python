# ApiResponseVecPlanDataInner

One canonical plan. `price_eur == -1.0` means custom pricing.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**features** | [**PlanFeatures**](PlanFeatures.md) |  | 
**id** | **str** |  | 
**limits** | [**PlanLimits**](PlanLimits.md) |  | 
**name** | **str** |  | 
**price_eur** | **float** |  | 

## Example

```python
from simplebilly_api.models.api_response_vec_plan_data_inner import ApiResponseVecPlanDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseVecPlanDataInner from a JSON string
api_response_vec_plan_data_inner_instance = ApiResponseVecPlanDataInner.from_json(json)
# print the JSON string representation of the object
print(ApiResponseVecPlanDataInner.to_json())

# convert the object into a dict
api_response_vec_plan_data_inner_dict = api_response_vec_plan_data_inner_instance.to_dict()
# create an instance of ApiResponseVecPlanDataInner from a dict
api_response_vec_plan_data_inner_from_dict = ApiResponseVecPlanDataInner.from_dict(api_response_vec_plan_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


