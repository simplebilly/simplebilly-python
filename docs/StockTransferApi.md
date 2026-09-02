# simplebilly_api.StockTransferApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_stock_transfer**](StockTransferApi.md#create_stock_transfer) | **POST** /api/v1/stock-transfers | 
[**delete_stock_transfer**](StockTransferApi.md#delete_stock_transfer) | **DELETE** /api/v1/stock-transfers/{stock_transfer_id} | 
[**get_stock_transfer**](StockTransferApi.md#get_stock_transfer) | **GET** /api/v1/stock-transfers/{stock_transfer_id} | 
[**list_stock_transfers**](StockTransferApi.md#list_stock_transfers) | **GET** /api/v1/stock-transfers/ | 
[**update_stock_transfer_status**](StockTransferApi.md#update_stock_transfer_status) | **PUT** /api/v1/stock-transfers/{stock_transfer_id}/status | 


# **create_stock_transfer**
> StockTransfer create_stock_transfer(stock_transfer)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.stock_transfer import StockTransfer
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
    api_instance = simplebilly_api.StockTransferApi(api_client)
    stock_transfer = simplebilly_api.StockTransfer() # StockTransfer | 

    try:
        api_response = api_instance.create_stock_transfer(stock_transfer)
        print("The response of StockTransferApi->create_stock_transfer:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StockTransferApi->create_stock_transfer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stock_transfer** | [**StockTransfer**](StockTransfer.md)|  | 

### Return type

[**StockTransfer**](StockTransfer.md)

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

# **delete_stock_transfer**
> delete_stock_transfer(stock_transfer_id)

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
    api_instance = simplebilly_api.StockTransferApi(api_client)
    stock_transfer_id = 'stock_transfer_id_example' # str | 

    try:
        api_instance.delete_stock_transfer(stock_transfer_id)
    except Exception as e:
        print("Exception when calling StockTransferApi->delete_stock_transfer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stock_transfer_id** | **str**|  | 

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

# **get_stock_transfer**
> StockTransfer get_stock_transfer(stock_transfer_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.stock_transfer import StockTransfer
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
    api_instance = simplebilly_api.StockTransferApi(api_client)
    stock_transfer_id = 'stock_transfer_id_example' # str | 

    try:
        api_response = api_instance.get_stock_transfer(stock_transfer_id)
        print("The response of StockTransferApi->get_stock_transfer:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StockTransferApi->get_stock_transfer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stock_transfer_id** | **str**|  | 

### Return type

[**StockTransfer**](StockTransfer.md)

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

# **list_stock_transfers**
> List[StockTransfer] list_stock_transfers(page=page, page_size=page_size, status=status, warehouse_id=warehouse_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.stock_transfer import StockTransfer
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
    api_instance = simplebilly_api.StockTransferApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    status = 'status_example' # str |  (optional)
    warehouse_id = 'warehouse_id_example' # str |  (optional)

    try:
        api_response = api_instance.list_stock_transfers(page=page, page_size=page_size, status=status, warehouse_id=warehouse_id)
        print("The response of StockTransferApi->list_stock_transfers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StockTransferApi->list_stock_transfers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **status** | **str**|  | [optional] 
 **warehouse_id** | **str**|  | [optional] 

### Return type

[**List[StockTransfer]**](StockTransfer.md)

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

# **update_stock_transfer_status**
> StockTransfer update_stock_transfer_status(stock_transfer_id, stock_transfer_status_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.stock_transfer import StockTransfer
from simplebilly_api.models.stock_transfer_status_update import StockTransferStatusUpdate
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
    api_instance = simplebilly_api.StockTransferApi(api_client)
    stock_transfer_id = 'stock_transfer_id_example' # str | 
    stock_transfer_status_update = simplebilly_api.StockTransferStatusUpdate() # StockTransferStatusUpdate | 

    try:
        api_response = api_instance.update_stock_transfer_status(stock_transfer_id, stock_transfer_status_update)
        print("The response of StockTransferApi->update_stock_transfer_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StockTransferApi->update_stock_transfer_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stock_transfer_id** | **str**|  | 
 **stock_transfer_status_update** | [**StockTransferStatusUpdate**](StockTransferStatusUpdate.md)|  | 

### Return type

[**StockTransfer**](StockTransfer.md)

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

