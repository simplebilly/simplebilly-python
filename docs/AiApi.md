# simplebilly_api.AiApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ai_suggest_api**](AiApi.md#ai_suggest_api) | **POST** /api/v1/support/ai/suggest | 
[**create_worker_api**](AiApi.md#create_worker_api) | **POST** /api/v1/support/ai/workers | 
[**list_workers_api**](AiApi.md#list_workers_api) | **GET** /api/v1/support/ai/workers | 
[**run_worker_api**](AiApi.md#run_worker_api) | **POST** /api/v1/support/ai/workers/{worker_id}/run | 


# **ai_suggest_api**
> AiSuggestion ai_suggest_api(ai_suggestion_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.ai_suggestion import AiSuggestion
from simplebilly_api.models.ai_suggestion_request import AiSuggestionRequest
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
    api_instance = simplebilly_api.AiApi(api_client)
    ai_suggestion_request = simplebilly_api.AiSuggestionRequest() # AiSuggestionRequest | 

    try:
        api_response = api_instance.ai_suggest_api(ai_suggestion_request)
        print("The response of AiApi->ai_suggest_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AiApi->ai_suggest_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ai_suggestion_request** | [**AiSuggestionRequest**](AiSuggestionRequest.md)|  | 

### Return type

[**AiSuggestion**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | AI suggestion |  -  |
**500** | AI error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_worker_api**
> AiWorkerConfig create_worker_api(ai_config_dto)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.ai_config_dto import AiConfigDto
from simplebilly_api.models.ai_worker_config import AiWorkerConfig
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
    api_instance = simplebilly_api.AiApi(api_client)
    ai_config_dto = simplebilly_api.AiConfigDto() # AiConfigDto | 

    try:
        api_response = api_instance.create_worker_api(ai_config_dto)
        print("The response of AiApi->create_worker_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AiApi->create_worker_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ai_config_dto** | [**AiConfigDto**](AiConfigDto.md)|  | 

### Return type

[**AiWorkerConfig**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Worker created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_workers_api**
> List[AiWorkerConfig] list_workers_api()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.ai_worker_config import AiWorkerConfig
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
    api_instance = simplebilly_api.AiApi(api_client)

    try:
        api_response = api_instance.list_workers_api()
        print("The response of AiApi->list_workers_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AiApi->list_workers_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[AiWorkerConfig]**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List AI workers |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **run_worker_api**
> AiSuggestion run_worker_api(worker_id, ai_suggestion_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.ai_suggestion import AiSuggestion
from simplebilly_api.models.ai_suggestion_request import AiSuggestionRequest
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
    api_instance = simplebilly_api.AiApi(api_client)
    worker_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    ai_suggestion_request = simplebilly_api.AiSuggestionRequest() # AiSuggestionRequest | 

    try:
        api_response = api_instance.run_worker_api(worker_id, ai_suggestion_request)
        print("The response of AiApi->run_worker_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AiApi->run_worker_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **worker_id** | **UUID**|  | 
 **ai_suggestion_request** | [**AiSuggestionRequest**](AiSuggestionRequest.md)|  | 

### Return type

[**AiSuggestion**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Worker executed |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

