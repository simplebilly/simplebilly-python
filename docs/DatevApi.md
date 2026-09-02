# simplebilly_api.DatevApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**datev_export_api**](DatevApi.md#datev_export_api) | **GET** /api/v1/bookkeeping/datev/export | Export bookkeeping data as DATEV CSV
[**datev_preview_api**](DatevApi.md#datev_preview_api) | **GET** /api/v1/bookkeeping/datev/preview | Exported_datev_bookings: returns formed bookings for review


# **datev_export_api**
> DatevExportResponse datev_export_api(account_schema=account_schema, date_from=date_from, date_to=date_to, page=page, page_size=page_size)

Export bookkeeping data as DATEV CSV

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.datev_export_response import DatevExportResponse
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
    api_instance = simplebilly_api.DatevApi(api_client)
    account_schema = 'account_schema_example' # str |  (optional)
    date_from = 'date_from_example' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)

    try:
        # Export bookkeeping data as DATEV CSV
        api_response = api_instance.datev_export_api(account_schema=account_schema, date_from=date_from, date_to=date_to, page=page, page_size=page_size)
        print("The response of DatevApi->datev_export_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatevApi->datev_export_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_schema** | **str**|  | [optional] 
 **date_from** | **str**|  | [optional] 
 **date_to** | **str**|  | [optional] 
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 

### Return type

[**DatevExportResponse**](DatevExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | DATEV CSV export |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **datev_preview_api**
> List[DatevBookingPreview] datev_preview_api(account_schema=account_schema, date_from=date_from, date_to=date_to, page=page, page_size=page_size)

Exported_datev_bookings: returns formed bookings for review

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.datev_booking_preview import DatevBookingPreview
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
    api_instance = simplebilly_api.DatevApi(api_client)
    account_schema = 'account_schema_example' # str |  (optional)
    date_from = 'date_from_example' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)

    try:
        # Exported_datev_bookings: returns formed bookings for review
        api_response = api_instance.datev_preview_api(account_schema=account_schema, date_from=date_from, date_to=date_to, page=page, page_size=page_size)
        print("The response of DatevApi->datev_preview_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatevApi->datev_preview_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_schema** | **str**|  | [optional] 
 **date_from** | **str**|  | [optional] 
 **date_to** | **str**|  | [optional] 
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 

### Return type

[**List[DatevBookingPreview]**](DatevBookingPreview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | DATEV booking preview |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

