# simplebilly_api.EmissionsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_emission_entry_api**](EmissionsApi.md#create_emission_entry_api) | **POST** /api/v1/bookkeeping/emissions/entries | 
[**create_emission_target_api**](EmissionsApi.md#create_emission_target_api) | **POST** /api/v1/bookkeeping/emissions/targets | 
[**delete_emission_entry_api**](EmissionsApi.md#delete_emission_entry_api) | **DELETE** /api/v1/bookkeeping/emissions/entries/{id} | 
[**delete_emission_target_api**](EmissionsApi.md#delete_emission_target_api) | **DELETE** /api/v1/bookkeeping/emissions/targets/{id} | 
[**emissions_entries_api**](EmissionsApi.md#emissions_entries_api) | **GET** /api/v1/bookkeeping/emissions/entries | 
[**emissions_export_api**](EmissionsApi.md#emissions_export_api) | **GET** /api/v1/bookkeeping/emissions/export | 
[**emissions_factors_api**](EmissionsApi.md#emissions_factors_api) | **GET** /api/v1/bookkeeping/emissions/factors | 
[**emissions_report_api**](EmissionsApi.md#emissions_report_api) | **GET** /api/v1/bookkeeping/emissions/report | 
[**emissions_targets_api**](EmissionsApi.md#emissions_targets_api) | **GET** /api/v1/bookkeeping/emissions/targets | 


# **create_emission_entry_api**
> EmissionEntry create_emission_entry_api(create_emission_entry)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.create_emission_entry import CreateEmissionEntry
from simplebilly_api.models.emission_entry import EmissionEntry
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
    api_instance = simplebilly_api.EmissionsApi(api_client)
    create_emission_entry = simplebilly_api.CreateEmissionEntry() # CreateEmissionEntry | 

    try:
        api_response = api_instance.create_emission_entry_api(create_emission_entry)
        print("The response of EmissionsApi->create_emission_entry_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmissionsApi->create_emission_entry_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_emission_entry** | [**CreateEmissionEntry**](CreateEmissionEntry.md)|  | 

### Return type

[**EmissionEntry**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Emission entry created |  -  |
**400** | Unknown category/method |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_emission_target_api**
> EmissionTarget create_emission_target_api(create_emission_target)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.create_emission_target import CreateEmissionTarget
from simplebilly_api.models.emission_target import EmissionTarget
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
    api_instance = simplebilly_api.EmissionsApi(api_client)
    create_emission_target = simplebilly_api.CreateEmissionTarget() # CreateEmissionTarget | 

    try:
        api_response = api_instance.create_emission_target_api(create_emission_target)
        print("The response of EmissionsApi->create_emission_target_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmissionsApi->create_emission_target_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_emission_target** | [**CreateEmissionTarget**](CreateEmissionTarget.md)|  | 

### Return type

[**EmissionTarget**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Emission target created |  -  |
**400** | Invalid scope |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_emission_entry_api**
> delete_emission_entry_api(id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
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
    api_instance = simplebilly_api.EmissionsApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_instance.delete_emission_entry_api(id)
    except Exception as e:
        print("Exception when calling EmissionsApi->delete_emission_entry_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

void (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Emission entry deleted |  -  |
**404** | Entry not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_emission_target_api**
> delete_emission_target_api(id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
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
    api_instance = simplebilly_api.EmissionsApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_instance.delete_emission_target_api(id)
    except Exception as e:
        print("Exception when calling EmissionsApi->delete_emission_target_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

void (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Emission target deleted |  -  |
**404** | Target not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **emissions_entries_api**
> List[EmissionEntry] emissions_entries_api(year)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.emission_entry import EmissionEntry
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
    api_instance = simplebilly_api.EmissionsApi(api_client)
    year = 56 # int | 

    try:
        api_response = api_instance.emissions_entries_api(year)
        print("The response of EmissionsApi->emissions_entries_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmissionsApi->emissions_entries_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**|  | 

### Return type

[**List[EmissionEntry]**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Emission entries for year |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **emissions_export_api**
> EmissionsExportResponse emissions_export_api(year)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.emissions_export_response import EmissionsExportResponse
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
    api_instance = simplebilly_api.EmissionsApi(api_client)
    year = 56 # int | 

    try:
        api_response = api_instance.emissions_export_api(year)
        print("The response of EmissionsApi->emissions_export_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmissionsApi->emissions_export_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**|  | 

### Return type

[**EmissionsExportResponse**](EmissionsExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Emissions CSV export |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **emissions_factors_api**
> List[EmissionFactorResponse] emissions_factors_api()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.emission_factor_response import EmissionFactorResponse
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
    api_instance = simplebilly_api.EmissionsApi(api_client)

    try:
        api_response = api_instance.emissions_factors_api()
        print("The response of EmissionsApi->emissions_factors_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmissionsApi->emissions_factors_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[EmissionFactorResponse]**](EmissionFactorResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Builtin emission factors |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **emissions_report_api**
> EmissionsReport emissions_report_api(year)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.emissions_report import EmissionsReport
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
    api_instance = simplebilly_api.EmissionsApi(api_client)
    year = 56 # int | 

    try:
        api_response = api_instance.emissions_report_api(year)
        print("The response of EmissionsApi->emissions_report_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmissionsApi->emissions_report_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**|  | 

### Return type

[**EmissionsReport**](EmissionsReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Emissions report |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **emissions_targets_api**
> List[EmissionTarget] emissions_targets_api()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.emission_target import EmissionTarget
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
    api_instance = simplebilly_api.EmissionsApi(api_client)

    try:
        api_response = api_instance.emissions_targets_api()
        print("The response of EmissionsApi->emissions_targets_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmissionsApi->emissions_targets_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[EmissionTarget]**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Emission reduction targets (ESRS E1-4) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

