# simplebilly_api.ReturnOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_return_order**](ReturnOrderApi.md#create_return_order) | **POST** /api/v1/returns | 
[**delete_return_order**](ReturnOrderApi.md#delete_return_order) | **DELETE** /api/v1/returns/{return_order_id} | 
[**get_return_order**](ReturnOrderApi.md#get_return_order) | **GET** /api/v1/returns/{return_order_id} | 
[**list_return_orders**](ReturnOrderApi.md#list_return_orders) | **GET** /api/v1/returns/ | 
[**return_logistics_queue**](ReturnOrderApi.md#return_logistics_queue) | **GET** /api/v1/returns/logistics-queue | 
[**return_logistics_summary**](ReturnOrderApi.md#return_logistics_summary) | **GET** /api/v1/returns/logistics-summary | Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.
[**update_return_order**](ReturnOrderApi.md#update_return_order) | **PUT** /api/v1/returns/{return_order_id} | 
[**update_return_order_status**](ReturnOrderApi.md#update_return_order_status) | **PUT** /api/v1/returns/{return_order_id}/status | 


# **create_return_order**
> ReturnOrder create_return_order(return_order)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.return_order import ReturnOrder
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
    api_instance = simplebilly_api.ReturnOrderApi(api_client)
    return_order = simplebilly_api.ReturnOrder() # ReturnOrder | 

    try:
        api_response = api_instance.create_return_order(return_order)
        print("The response of ReturnOrderApi->create_return_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReturnOrderApi->create_return_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_order** | [**ReturnOrder**](ReturnOrder.md)|  | 

### Return type

[**ReturnOrder**](ReturnOrder.md)

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

# **delete_return_order**
> delete_return_order(return_order_id)

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
    api_instance = simplebilly_api.ReturnOrderApi(api_client)
    return_order_id = 'return_order_id_example' # str | 

    try:
        api_instance.delete_return_order(return_order_id)
    except Exception as e:
        print("Exception when calling ReturnOrderApi->delete_return_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_order_id** | **str**|  | 

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
**400** | Bad request |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_return_order**
> ReturnOrder get_return_order(return_order_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.return_order import ReturnOrder
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
    api_instance = simplebilly_api.ReturnOrderApi(api_client)
    return_order_id = 'return_order_id_example' # str | 

    try:
        api_response = api_instance.get_return_order(return_order_id)
        print("The response of ReturnOrderApi->get_return_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReturnOrderApi->get_return_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_order_id** | **str**|  | 

### Return type

[**ReturnOrder**](ReturnOrder.md)

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

# **list_return_orders**
> List[ReturnOrder] list_return_orders(page=page, page_size=page_size, status=status, customer_name=customer_name, order_number=order_number)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.return_order import ReturnOrder
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
    api_instance = simplebilly_api.ReturnOrderApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    status = 'status_example' # str |  (optional)
    customer_name = 'customer_name_example' # str |  (optional)
    order_number = 'order_number_example' # str |  (optional)

    try:
        api_response = api_instance.list_return_orders(page=page, page_size=page_size, status=status, customer_name=customer_name, order_number=order_number)
        print("The response of ReturnOrderApi->list_return_orders:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReturnOrderApi->list_return_orders: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **status** | **str**|  | [optional] 
 **customer_name** | **str**|  | [optional] 
 **order_number** | **str**|  | [optional] 

### Return type

[**List[ReturnOrder]**](ReturnOrder.md)

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

# **return_logistics_queue**
> List[ReturnLogisticsQueueItem] return_logistics_queue()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.return_logistics_queue_item import ReturnLogisticsQueueItem
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
    api_instance = simplebilly_api.ReturnOrderApi(api_client)

    try:
        api_response = api_instance.return_logistics_queue()
        print("The response of ReturnOrderApi->return_logistics_queue:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReturnOrderApi->return_logistics_queue: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[ReturnLogisticsQueueItem]**](ReturnLogisticsQueueItem.md)

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

# **return_logistics_summary**
> ReturnLogisticsSummary return_logistics_summary()

Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.return_logistics_summary import ReturnLogisticsSummary
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
    api_instance = simplebilly_api.ReturnOrderApi(api_client)

    try:
        # Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.
        api_response = api_instance.return_logistics_summary()
        print("The response of ReturnOrderApi->return_logistics_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReturnOrderApi->return_logistics_summary: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ReturnLogisticsSummary**](ReturnLogisticsSummary.md)

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

# **update_return_order**
> ReturnOrder update_return_order(return_order_id, body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.return_order import ReturnOrder
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
    api_instance = simplebilly_api.ReturnOrderApi(api_client)
    return_order_id = 'return_order_id_example' # str | 
    body = None # object | 

    try:
        api_response = api_instance.update_return_order(return_order_id, body)
        print("The response of ReturnOrderApi->update_return_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReturnOrderApi->update_return_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_order_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**ReturnOrder**](ReturnOrder.md)

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

# **update_return_order_status**
> ReturnOrder update_return_order_status(return_order_id, return_order_status_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.return_order import ReturnOrder
from simplebilly_api.models.return_order_status_update import ReturnOrderStatusUpdate
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
    api_instance = simplebilly_api.ReturnOrderApi(api_client)
    return_order_id = 'return_order_id_example' # str | 
    return_order_status_update = simplebilly_api.ReturnOrderStatusUpdate() # ReturnOrderStatusUpdate | 

    try:
        api_response = api_instance.update_return_order_status(return_order_id, return_order_status_update)
        print("The response of ReturnOrderApi->update_return_order_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReturnOrderApi->update_return_order_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_order_id** | **str**|  | 
 **return_order_status_update** | [**ReturnOrderStatusUpdate**](ReturnOrderStatusUpdate.md)|  | 

### Return type

[**ReturnOrder**](ReturnOrder.md)

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

