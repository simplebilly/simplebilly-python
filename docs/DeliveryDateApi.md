# simplebilly_api.DeliveryDateApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_delivery_date**](DeliveryDateApi.md#create_delivery_date) | **POST** /api/v1/delivery-dates | 
[**delete_delivery_date**](DeliveryDateApi.md#delete_delivery_date) | **DELETE** /api/v1/delivery-dates/{delivery_date_id} | 
[**get_delivery_date**](DeliveryDateApi.md#get_delivery_date) | **GET** /api/v1/delivery-dates/{delivery_date_id} | 
[**get_delivery_performance**](DeliveryDateApi.md#get_delivery_performance) | **GET** /api/v1/delivery-dates/performance | On-time performance summary: how many promised delivery dates were met within a period.
[**list_delivery_dates**](DeliveryDateApi.md#list_delivery_dates) | **GET** /api/v1/delivery-dates/ | 
[**update_delivery_date**](DeliveryDateApi.md#update_delivery_date) | **PUT** /api/v1/delivery-dates/{delivery_date_id} | 
[**update_delivery_date_status**](DeliveryDateApi.md#update_delivery_date_status) | **PUT** /api/v1/delivery-dates/{delivery_date_id}/status | 


# **create_delivery_date**
> DeliveryDate create_delivery_date(delivery_date_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.delivery_date import DeliveryDate
from simplebilly_api.models.delivery_date_create import DeliveryDateCreate
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
    api_instance = simplebilly_api.DeliveryDateApi(api_client)
    delivery_date_create = simplebilly_api.DeliveryDateCreate() # DeliveryDateCreate | 

    try:
        api_response = api_instance.create_delivery_date(delivery_date_create)
        print("The response of DeliveryDateApi->create_delivery_date:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryDateApi->create_delivery_date: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **delivery_date_create** | [**DeliveryDateCreate**](DeliveryDateCreate.md)|  | 

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | Bad request |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_delivery_date**
> delete_delivery_date(delivery_date_id)

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
    api_instance = simplebilly_api.DeliveryDateApi(api_client)
    delivery_date_id = 'delivery_date_id_example' # str | 

    try:
        api_instance.delete_delivery_date(delivery_date_id)
    except Exception as e:
        print("Exception when calling DeliveryDateApi->delete_delivery_date: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **delivery_date_id** | **str**|  | 

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
**204** | No Content |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_delivery_date**
> DeliveryDate get_delivery_date(delivery_date_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.delivery_date import DeliveryDate
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
    api_instance = simplebilly_api.DeliveryDateApi(api_client)
    delivery_date_id = 'delivery_date_id_example' # str | 

    try:
        api_response = api_instance.get_delivery_date(delivery_date_id)
        print("The response of DeliveryDateApi->get_delivery_date:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryDateApi->get_delivery_date: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **delivery_date_id** | **str**|  | 

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_delivery_performance**
> object get_delivery_performance(page=page, page_size=page_size, order_number=order_number, status=status, var_from=var_from, to=to)

On-time performance summary: how many promised delivery dates were met within a period.

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
    api_instance = simplebilly_api.DeliveryDateApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    order_number = 'order_number_example' # str |  (optional)
    status = 'status_example' # str |  (optional)
    var_from = '2013-10-20' # date | Only dates on or after this date. (optional)
    to = '2013-10-20' # date | Only dates on or before this date. (optional)

    try:
        # On-time performance summary: how many promised delivery dates were met within a period.
        api_response = api_instance.get_delivery_performance(page=page, page_size=page_size, order_number=order_number, status=status, var_from=var_from, to=to)
        print("The response of DeliveryDateApi->get_delivery_performance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryDateApi->get_delivery_performance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **order_number** | **str**|  | [optional] 
 **status** | **str**|  | [optional] 
 **var_from** | **date**| Only dates on or after this date. | [optional] 
 **to** | **date**| Only dates on or before this date. | [optional] 

### Return type

**object**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_delivery_dates**
> List[DeliveryDate] list_delivery_dates(page=page, page_size=page_size, order_number=order_number, status=status, var_from=var_from, to=to)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.delivery_date import DeliveryDate
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
    api_instance = simplebilly_api.DeliveryDateApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    order_number = 'order_number_example' # str |  (optional)
    status = 'status_example' # str |  (optional)
    var_from = '2013-10-20' # date | Only dates on or after this date. (optional)
    to = '2013-10-20' # date | Only dates on or before this date. (optional)

    try:
        api_response = api_instance.list_delivery_dates(page=page, page_size=page_size, order_number=order_number, status=status, var_from=var_from, to=to)
        print("The response of DeliveryDateApi->list_delivery_dates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryDateApi->list_delivery_dates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **order_number** | **str**|  | [optional] 
 **status** | **str**|  | [optional] 
 **var_from** | **date**| Only dates on or after this date. | [optional] 
 **to** | **date**| Only dates on or before this date. | [optional] 

### Return type

[**List[DeliveryDate]**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_delivery_date**
> DeliveryDate update_delivery_date(delivery_date_id, body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.delivery_date import DeliveryDate
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
    api_instance = simplebilly_api.DeliveryDateApi(api_client)
    delivery_date_id = 'delivery_date_id_example' # str | 
    body = None # object | 

    try:
        api_response = api_instance.update_delivery_date(delivery_date_id, body)
        print("The response of DeliveryDateApi->update_delivery_date:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryDateApi->update_delivery_date: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **delivery_date_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad request |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_delivery_date_status**
> DeliveryDate update_delivery_date_status(delivery_date_id, delivery_date_status_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.delivery_date import DeliveryDate
from simplebilly_api.models.delivery_date_status_update import DeliveryDateStatusUpdate
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
    api_instance = simplebilly_api.DeliveryDateApi(api_client)
    delivery_date_id = 'delivery_date_id_example' # str | 
    delivery_date_status_update = simplebilly_api.DeliveryDateStatusUpdate() # DeliveryDateStatusUpdate | 

    try:
        api_response = api_instance.update_delivery_date_status(delivery_date_id, delivery_date_status_update)
        print("The response of DeliveryDateApi->update_delivery_date_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryDateApi->update_delivery_date_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **delivery_date_id** | **str**|  | 
 **delivery_date_status_update** | [**DeliveryDateStatusUpdate**](DeliveryDateStatusUpdate.md)|  | 

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad request |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

