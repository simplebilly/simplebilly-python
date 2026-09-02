# simplebilly_api.BudgetsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**budgets_api**](BudgetsApi.md#budgets_api) | **GET** /api/v1/bookkeeping/budgets | 
[**upsert_budget_goal_api**](BudgetsApi.md#upsert_budget_goal_api) | **PUT** /api/v1/bookkeeping/budgets/goals/{category} | 


# **budgets_api**
> BudgetErgebnis budgets_api(year, month)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.budget_ergebnis import BudgetErgebnis
from simplebilly_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://demo.simplebilly.com
# See configuration.py for a list of all supported configuration parameters.
configuration = simplebilly_api.Configuration(
    host = "https://demo.simplebilly.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearer_token
configuration = simplebilly_api.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with simplebilly_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = simplebilly_api.BudgetsApi(api_client)
    year = 56 # int | 
    month = 56 # int | 

    try:
        api_response = api_instance.budgets_api(year, month)
        print("The response of BudgetsApi->budgets_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BudgetsApi->budgets_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**|  | 
 **month** | **int**|  | 

### Return type

[**BudgetErgebnis**](BudgetErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Monats-Budget + Prognose |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upsert_budget_goal_api**
> Budget upsert_budget_goal_api(category, budget_goal_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.budget import Budget
from simplebilly_api.models.budget_goal_request import BudgetGoalRequest
from simplebilly_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://demo.simplebilly.com
# See configuration.py for a list of all supported configuration parameters.
configuration = simplebilly_api.Configuration(
    host = "https://demo.simplebilly.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearer_token
configuration = simplebilly_api.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with simplebilly_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = simplebilly_api.BudgetsApi(api_client)
    category = 'category_example' # str | 
    budget_goal_request = simplebilly_api.BudgetGoalRequest() # BudgetGoalRequest | 

    try:
        api_response = api_instance.upsert_budget_goal_api(category, budget_goal_request)
        print("The response of BudgetsApi->upsert_budget_goal_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BudgetsApi->upsert_budget_goal_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category** | **str**|  | 
 **budget_goal_request** | [**BudgetGoalRequest**](BudgetGoalRequest.md)|  | 

### Return type

[**Budget**](Budget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Budget goal saved (upsert) |  -  |
**400** | Negative goal |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

