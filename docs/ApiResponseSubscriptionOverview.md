# ApiResponseSubscriptionOverview


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ApiResponseSubscriptionOverviewData**](ApiResponseSubscriptionOverviewData.md) |  | [optional] 
**error** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.api_response_subscription_overview import ApiResponseSubscriptionOverview

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseSubscriptionOverview from a JSON string
api_response_subscription_overview_instance = ApiResponseSubscriptionOverview.from_json(json)
# print the JSON string representation of the object
print(ApiResponseSubscriptionOverview.to_json())

# convert the object into a dict
api_response_subscription_overview_dict = api_response_subscription_overview_instance.to_dict()
# create an instance of ApiResponseSubscriptionOverview from a dict
api_response_subscription_overview_from_dict = ApiResponseSubscriptionOverview.from_dict(api_response_subscription_overview_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


