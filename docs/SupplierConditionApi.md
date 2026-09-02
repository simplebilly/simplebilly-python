# simplebilly_api.SupplierConditionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_supplier_condition**](SupplierConditionApi.md#create_supplier_condition) | **POST** /api/v1/supplier-conditions | 
[**delete_supplier_condition**](SupplierConditionApi.md#delete_supplier_condition) | **DELETE** /api/v1/supplier-conditions/{supplier_condition_id} | 
[**get_supplier_condition**](SupplierConditionApi.md#get_supplier_condition) | **GET** /api/v1/supplier-conditions/{supplier_condition_id} | 
[**list_supplier_conditions**](SupplierConditionApi.md#list_supplier_conditions) | **GET** /api/v1/supplier-conditions/ | 
[**update_supplier_condition**](SupplierConditionApi.md#update_supplier_condition) | **PUT** /api/v1/supplier-conditions/{supplier_condition_id} | 


# **create_supplier_condition**
> SupplierCondition create_supplier_condition(supplier_condition_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.supplier_condition import SupplierCondition
from simplebilly_api.models.supplier_condition_create import SupplierConditionCreate
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
    api_instance = simplebilly_api.SupplierConditionApi(api_client)
    supplier_condition_create = simplebilly_api.SupplierConditionCreate() # SupplierConditionCreate | 

    try:
        api_response = api_instance.create_supplier_condition(supplier_condition_create)
        print("The response of SupplierConditionApi->create_supplier_condition:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupplierConditionApi->create_supplier_condition: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplier_condition_create** | [**SupplierConditionCreate**](SupplierConditionCreate.md)|  | 

### Return type

[**SupplierCondition**](SupplierCondition.md)

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

# **delete_supplier_condition**
> delete_supplier_condition(supplier_condition_id)

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
    api_instance = simplebilly_api.SupplierConditionApi(api_client)
    supplier_condition_id = 'supplier_condition_id_example' # str | 

    try:
        api_instance.delete_supplier_condition(supplier_condition_id)
    except Exception as e:
        print("Exception when calling SupplierConditionApi->delete_supplier_condition: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplier_condition_id** | **str**|  | 

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

# **get_supplier_condition**
> SupplierCondition get_supplier_condition(supplier_condition_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.supplier_condition import SupplierCondition
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
    api_instance = simplebilly_api.SupplierConditionApi(api_client)
    supplier_condition_id = 'supplier_condition_id_example' # str | 

    try:
        api_response = api_instance.get_supplier_condition(supplier_condition_id)
        print("The response of SupplierConditionApi->get_supplier_condition:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupplierConditionApi->get_supplier_condition: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplier_condition_id** | **str**|  | 

### Return type

[**SupplierCondition**](SupplierCondition.md)

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

# **list_supplier_conditions**
> List[SupplierCondition] list_supplier_conditions(page=page, page_size=page_size, supplier_contact_id=supplier_contact_id, search=search)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.supplier_condition import SupplierCondition
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
    api_instance = simplebilly_api.SupplierConditionApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    supplier_contact_id = 'supplier_contact_id_example' # str |  (optional)
    search = 'search_example' # str |  (optional)

    try:
        api_response = api_instance.list_supplier_conditions(page=page, page_size=page_size, supplier_contact_id=supplier_contact_id, search=search)
        print("The response of SupplierConditionApi->list_supplier_conditions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupplierConditionApi->list_supplier_conditions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **supplier_contact_id** | **str**|  | [optional] 
 **search** | **str**|  | [optional] 

### Return type

[**List[SupplierCondition]**](SupplierCondition.md)

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

# **update_supplier_condition**
> SupplierCondition update_supplier_condition(supplier_condition_id, supplier_condition_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.supplier_condition import SupplierCondition
from simplebilly_api.models.supplier_condition_update import SupplierConditionUpdate
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
    api_instance = simplebilly_api.SupplierConditionApi(api_client)
    supplier_condition_id = 'supplier_condition_id_example' # str | 
    supplier_condition_update = simplebilly_api.SupplierConditionUpdate() # SupplierConditionUpdate | 

    try:
        api_response = api_instance.update_supplier_condition(supplier_condition_id, supplier_condition_update)
        print("The response of SupplierConditionApi->update_supplier_condition:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupplierConditionApi->update_supplier_condition: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplier_condition_id** | **str**|  | 
 **supplier_condition_update** | [**SupplierConditionUpdate**](SupplierConditionUpdate.md)|  | 

### Return type

[**SupplierCondition**](SupplierCondition.md)

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

