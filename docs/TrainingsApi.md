# simplebilly_api.TrainingsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_my_trainings**](TrainingsApi.md#get_my_trainings) | **GET** /api/v1/trainings/me | 
[**get_training_content**](TrainingsApi.md#get_training_content) | **GET** /api/v1/trainings/content/{code} | 
[**get_training_overview**](TrainingsApi.md#get_training_overview) | **GET** /api/v1/trainings/overview | 
[**submit_training_result**](TrainingsApi.md#submit_training_result) | **POST** /api/v1/trainings/submit-result | 


# **get_my_trainings**
> List[MyTrainingItem] get_my_trainings()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.my_training_item import MyTrainingItem
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
    api_instance = simplebilly_api.TrainingsApi(api_client)

    try:
        api_response = api_instance.get_my_trainings()
        print("The response of TrainingsApi->get_my_trainings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TrainingsApi->get_my_trainings: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[MyTrainingItem]**](MyTrainingItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Required trainings for the current employee |  -  |
**404** | No employee linked to user |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_training_content**
> TrainingContent get_training_content(code)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.training_content import TrainingContent
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
    api_instance = simplebilly_api.TrainingsApi(api_client)
    code = 'code_example' # str | Training code, e.g. data_privacy

    try:
        api_response = api_instance.get_training_content(code)
        print("The response of TrainingsApi->get_training_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TrainingsApi->get_training_content: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **str**| Training code, e.g. data_privacy | 

### Return type

[**TrainingContent**](TrainingContent.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Interactive training content for the frontend player |  -  |
**404** | Unknown training code |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_training_overview**
> List[HrTrainingOverview] get_training_overview()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.hr_training_overview import HrTrainingOverview
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
    api_instance = simplebilly_api.TrainingsApi(api_client)

    try:
        api_response = api_instance.get_training_overview()
        print("The response of TrainingsApi->get_training_overview:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TrainingsApi->get_training_overview: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[HrTrainingOverview]**](HrTrainingOverview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | HR overview of assigned trainings |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **submit_training_result**
> SubmitResultResponse submit_training_result(submit_result_dto)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.submit_result_dto import SubmitResultDto
from simplebilly_api.models.submit_result_response import SubmitResultResponse
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
    api_instance = simplebilly_api.TrainingsApi(api_client)
    submit_result_dto = simplebilly_api.SubmitResultDto() # SubmitResultDto | 

    try:
        api_response = api_instance.submit_training_result(submit_result_dto)
        print("The response of TrainingsApi->submit_training_result:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TrainingsApi->submit_training_result: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **submit_result_dto** | [**SubmitResultDto**](SubmitResultDto.md)|  | 

### Return type

[**SubmitResultResponse**](SubmitResultResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Result recorded |  -  |
**400** | Invalid score or training |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

