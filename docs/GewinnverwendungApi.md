# simplebilly_api.GewinnverwendungApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gewinnverwendung_api**](GewinnverwendungApi.md#gewinnverwendung_api) | **GET** /api/v1/bookkeeping/gewinnverwendung | 
[**gewinnverwendung_export_api**](GewinnverwendungApi.md#gewinnverwendung_export_api) | **GET** /api/v1/bookkeeping/gewinnverwendung/export | 


# **gewinnverwendung_api**
> GewinnverwendungsReport gewinnverwendung_api(year)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.gewinnverwendungs_report import GewinnverwendungsReport
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
    api_instance = simplebilly_api.GewinnverwendungApi(api_client)
    year = 56 # int | 

    try:
        api_response = api_instance.gewinnverwendung_api(year)
        print("The response of GewinnverwendungApi->gewinnverwendung_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GewinnverwendungApi->gewinnverwendung_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**|  | 

### Return type

[**GewinnverwendungsReport**](GewinnverwendungsReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Gewinnverwendungsrechnung (§ 150, § 174 AktG) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **gewinnverwendung_export_api**
> GewinnverwendungsExportResponse gewinnverwendung_export_api(year)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.gewinnverwendungs_export_response import GewinnverwendungsExportResponse
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
    api_instance = simplebilly_api.GewinnverwendungApi(api_client)
    year = 56 # int | 

    try:
        api_response = api_instance.gewinnverwendung_export_api(year)
        print("The response of GewinnverwendungApi->gewinnverwendung_export_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GewinnverwendungApi->gewinnverwendung_export_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**|  | 

### Return type

[**GewinnverwendungsExportResponse**](GewinnverwendungsExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Gewinnverwendungsrechnung als CSV (BOM, Semikolon) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

