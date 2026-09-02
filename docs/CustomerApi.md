# simplebilly_api.CustomerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_customer**](CustomerApi.md#create_customer) | **POST** /api/v1/customers | 
[**customer_restore**](CustomerApi.md#customer_restore) | **POST** /api/v1/customers/{customer_id}/restore | 
[**delete_customer**](CustomerApi.md#delete_customer) | **DELETE** /api/v1/customers/{customer_id} | 
[**get_customer**](CustomerApi.md#get_customer) | **GET** /api/v1/customers/{customer_id} | 
[**get_customers**](CustomerApi.md#get_customers) | **GET** /api/v1/customers/ | 
[**update_customer**](CustomerApi.md#update_customer) | **PUT** /api/v1/customers/{customer_id} | 


# **create_customer**
> Customer create_customer(customer_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer import Customer
from simplebilly_api.models.customer_create import CustomerCreate
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
    api_instance = simplebilly_api.CustomerApi(api_client)
    customer_create = simplebilly_api.CustomerCreate() # CustomerCreate | 

    try:
        api_response = api_instance.create_customer(customer_create)
        print("The response of CustomerApi->create_customer:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerApi->create_customer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_create** | [**CustomerCreate**](CustomerCreate.md)|  | 

### Return type

[**Customer**](Customer.md)

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

# **customer_restore**
> Customer customer_restore(customer_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer import Customer
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
    api_instance = simplebilly_api.CustomerApi(api_client)
    customer_id = 'customer_id_example' # str | 

    try:
        api_response = api_instance.customer_restore(customer_id)
        print("The response of CustomerApi->customer_restore:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerApi->customer_restore: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**|  | 

### Return type

[**Customer**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Restored |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_customer**
> delete_customer(customer_id)

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
    api_instance = simplebilly_api.CustomerApi(api_client)
    customer_id = 'customer_id_example' # str | 

    try:
        api_instance.delete_customer(customer_id)
    except Exception as e:
        print("Exception when calling CustomerApi->delete_customer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**|  | 

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

# **get_customer**
> Customer get_customer(customer_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer import Customer
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
    api_instance = simplebilly_api.CustomerApi(api_client)
    customer_id = 'customer_id_example' # str | 

    try:
        api_response = api_instance.get_customer(customer_id)
        print("The response of CustomerApi->get_customer:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerApi->get_customer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**|  | 

### Return type

[**Customer**](Customer.md)

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

# **get_customers**
> List[Customer] get_customers(page=page, page_size=page_size, search=search, include_deleted=include_deleted)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer import Customer
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
    api_instance = simplebilly_api.CustomerApi(api_client)
    page = 1 # int |  (optional)
    page_size = 56 # int |  (optional)
    search = 'search_example' # str |  (optional)
    include_deleted = True # bool | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)

    try:
        api_response = api_instance.get_customers(page=page, page_size=page_size, search=search, include_deleted=include_deleted)
        print("The response of CustomerApi->get_customers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerApi->get_customers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **search** | **str**|  | [optional] 
 **include_deleted** | **bool**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] 

### Return type

[**List[Customer]**](Customer.md)

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

# **update_customer**
> Customer update_customer(customer_id, customer_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer import Customer
from simplebilly_api.models.customer_update import CustomerUpdate
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
    api_instance = simplebilly_api.CustomerApi(api_client)
    customer_id = 'customer_id_example' # str | 
    customer_update = simplebilly_api.CustomerUpdate() # CustomerUpdate | 

    try:
        api_response = api_instance.update_customer(customer_id, customer_update)
        print("The response of CustomerApi->update_customer:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerApi->update_customer: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**|  | 
 **customer_update** | [**CustomerUpdate**](CustomerUpdate.md)|  | 

### Return type

[**Customer**](Customer.md)

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

