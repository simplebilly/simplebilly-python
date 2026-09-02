# simplebilly_api.DeclarationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_declaration**](DeclarationApi.md#create_declaration) | **POST** /api/v1/declarations | 
[**declaration_restore**](DeclarationApi.md#declaration_restore) | **POST** /api/v1/declarations/{id}/restore | 
[**delete_declaration**](DeclarationApi.md#delete_declaration) | **DELETE** /api/v1/declarations/{id} | 
[**get_declaration**](DeclarationApi.md#get_declaration) | **GET** /api/v1/declarations/{id} | 
[**get_declarations**](DeclarationApi.md#get_declarations) | **GET** /api/v1/declarations/ | 
[**update_declaration**](DeclarationApi.md#update_declaration) | **PUT** /api/v1/declarations/{id} | 


# **create_declaration**
> Declaration create_declaration(declaration_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.declaration import Declaration
from simplebilly_api.models.declaration_create import DeclarationCreate
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
    api_instance = simplebilly_api.DeclarationApi(api_client)
    declaration_create = simplebilly_api.DeclarationCreate() # DeclarationCreate | 

    try:
        api_response = api_instance.create_declaration(declaration_create)
        print("The response of DeclarationApi->create_declaration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeclarationApi->create_declaration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **declaration_create** | [**DeclarationCreate**](DeclarationCreate.md)|  | 

### Return type

[**Declaration**](Declaration.md)

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

# **declaration_restore**
> Declaration declaration_restore(id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.declaration import Declaration
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
    api_instance = simplebilly_api.DeclarationApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_response = api_instance.declaration_restore(id)
        print("The response of DeclarationApi->declaration_restore:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeclarationApi->declaration_restore: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

[**Declaration**](Declaration.md)

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

# **delete_declaration**
> delete_declaration(id)

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
    api_instance = simplebilly_api.DeclarationApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_instance.delete_declaration(id)
    except Exception as e:
        print("Exception when calling DeclarationApi->delete_declaration: %s\n" % e)
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
**204** | No Content |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_declaration**
> Declaration get_declaration(id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.declaration import Declaration
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
    api_instance = simplebilly_api.DeclarationApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_response = api_instance.get_declaration(id)
        print("The response of DeclarationApi->get_declaration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeclarationApi->get_declaration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 

### Return type

[**Declaration**](Declaration.md)

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

# **get_declarations**
> List[Declaration] get_declarations(page=page, page_size=page_size, search=search, include_deleted=include_deleted)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.declaration import Declaration
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
    api_instance = simplebilly_api.DeclarationApi(api_client)
    page = 1 # int |  (optional)
    page_size = 56 # int |  (optional)
    search = 'search_example' # str |  (optional)
    include_deleted = True # bool | Soft-delete entities: set true to include rows with `deleted_at` set. (optional)

    try:
        api_response = api_instance.get_declarations(page=page, page_size=page_size, search=search, include_deleted=include_deleted)
        print("The response of DeclarationApi->get_declarations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeclarationApi->get_declarations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **search** | **str**|  | [optional] 
 **include_deleted** | **bool**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] 

### Return type

[**List[Declaration]**](Declaration.md)

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

# **update_declaration**
> Declaration update_declaration(id, declaration_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.declaration import Declaration
from simplebilly_api.models.declaration_update import DeclarationUpdate
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
    api_instance = simplebilly_api.DeclarationApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    declaration_update = simplebilly_api.DeclarationUpdate() # DeclarationUpdate | 

    try:
        api_response = api_instance.update_declaration(id, declaration_update)
        print("The response of DeclarationApi->update_declaration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeclarationApi->update_declaration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **declaration_update** | [**DeclarationUpdate**](DeclarationUpdate.md)|  | 

### Return type

[**Declaration**](Declaration.md)

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

