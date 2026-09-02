# simplebilly_api.InventoryCountApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_inventory_count**](InventoryCountApi.md#create_inventory_count) | **POST** /api/v1/inventory-counts | 
[**delete_inventory_count**](InventoryCountApi.md#delete_inventory_count) | **DELETE** /api/v1/inventory-counts/{inventory_count_id} | 
[**generate_inventory_count**](InventoryCountApi.md#generate_inventory_count) | **POST** /api/v1/inventory-counts/generate | 
[**get_inventory_count**](InventoryCountApi.md#get_inventory_count) | **GET** /api/v1/inventory-counts/{inventory_count_id} | 
[**list_inventory_counts**](InventoryCountApi.md#list_inventory_counts) | **GET** /api/v1/inventory-counts/ | 
[**update_inventory_count**](InventoryCountApi.md#update_inventory_count) | **PUT** /api/v1/inventory-counts/{inventory_count_id} | 
[**update_inventory_count_status**](InventoryCountApi.md#update_inventory_count_status) | **PUT** /api/v1/inventory-counts/{inventory_count_id}/status | 


# **create_inventory_count**
> InventoryCount create_inventory_count(inventory_count)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.inventory_count import InventoryCount
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
    api_instance = simplebilly_api.InventoryCountApi(api_client)
    inventory_count = simplebilly_api.InventoryCount() # InventoryCount | 

    try:
        api_response = api_instance.create_inventory_count(inventory_count)
        print("The response of InventoryCountApi->create_inventory_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InventoryCountApi->create_inventory_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventory_count** | [**InventoryCount**](InventoryCount.md)|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

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

# **delete_inventory_count**
> delete_inventory_count(inventory_count_id)

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
    api_instance = simplebilly_api.InventoryCountApi(api_client)
    inventory_count_id = 'inventory_count_id_example' # str | 

    try:
        api_instance.delete_inventory_count(inventory_count_id)
    except Exception as e:
        print("Exception when calling InventoryCountApi->delete_inventory_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventory_count_id** | **str**|  | 

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

# **generate_inventory_count**
> InventoryCount generate_inventory_count(generate_count_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.generate_count_request import GenerateCountRequest
from simplebilly_api.models.inventory_count import InventoryCount
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
    api_instance = simplebilly_api.InventoryCountApi(api_client)
    generate_count_request = simplebilly_api.GenerateCountRequest() # GenerateCountRequest | 

    try:
        api_response = api_instance.generate_inventory_count(generate_count_request)
        print("The response of InventoryCountApi->generate_inventory_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InventoryCountApi->generate_inventory_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **generate_count_request** | [**GenerateCountRequest**](GenerateCountRequest.md)|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

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

# **get_inventory_count**
> InventoryCount get_inventory_count(inventory_count_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.inventory_count import InventoryCount
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
    api_instance = simplebilly_api.InventoryCountApi(api_client)
    inventory_count_id = 'inventory_count_id_example' # str | 

    try:
        api_response = api_instance.get_inventory_count(inventory_count_id)
        print("The response of InventoryCountApi->get_inventory_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InventoryCountApi->get_inventory_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventory_count_id** | **str**|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

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

# **list_inventory_counts**
> List[InventoryCount] list_inventory_counts(page=page, page_size=page_size, status=status, warehouse_id=warehouse_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.inventory_count import InventoryCount
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
    api_instance = simplebilly_api.InventoryCountApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    status = 'status_example' # str |  (optional)
    warehouse_id = 'warehouse_id_example' # str |  (optional)

    try:
        api_response = api_instance.list_inventory_counts(page=page, page_size=page_size, status=status, warehouse_id=warehouse_id)
        print("The response of InventoryCountApi->list_inventory_counts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InventoryCountApi->list_inventory_counts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **status** | **str**|  | [optional] 
 **warehouse_id** | **str**|  | [optional] 

### Return type

[**List[InventoryCount]**](InventoryCount.md)

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

# **update_inventory_count**
> InventoryCount update_inventory_count(inventory_count_id, body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.inventory_count import InventoryCount
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
    api_instance = simplebilly_api.InventoryCountApi(api_client)
    inventory_count_id = 'inventory_count_id_example' # str | 
    body = None # object | 

    try:
        api_response = api_instance.update_inventory_count(inventory_count_id, body)
        print("The response of InventoryCountApi->update_inventory_count:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InventoryCountApi->update_inventory_count: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventory_count_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

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

# **update_inventory_count_status**
> InventoryCount update_inventory_count_status(inventory_count_id, inventory_count_status_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.inventory_count import InventoryCount
from simplebilly_api.models.inventory_count_status_update import InventoryCountStatusUpdate
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
    api_instance = simplebilly_api.InventoryCountApi(api_client)
    inventory_count_id = 'inventory_count_id_example' # str | 
    inventory_count_status_update = simplebilly_api.InventoryCountStatusUpdate() # InventoryCountStatusUpdate | 

    try:
        api_response = api_instance.update_inventory_count_status(inventory_count_id, inventory_count_status_update)
        print("The response of InventoryCountApi->update_inventory_count_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InventoryCountApi->update_inventory_count_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventory_count_id** | **str**|  | 
 **inventory_count_status_update** | [**InventoryCountStatusUpdate**](InventoryCountStatusUpdate.md)|  | 

### Return type

[**InventoryCount**](InventoryCount.md)

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

