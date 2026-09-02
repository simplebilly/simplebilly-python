# simplebilly_api.ProductAttributeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_product_attribute**](ProductAttributeApi.md#create_product_attribute) | **POST** /api/v1/product-attributes | 
[**delete_product_attribute**](ProductAttributeApi.md#delete_product_attribute) | **DELETE** /api/v1/product-attributes/{attribute_id} | 
[**get_product_attribute**](ProductAttributeApi.md#get_product_attribute) | **GET** /api/v1/product-attributes/{attribute_id} | 
[**list_product_attributes**](ProductAttributeApi.md#list_product_attributes) | **GET** /api/v1/product-attributes/ | 
[**update_product_attribute**](ProductAttributeApi.md#update_product_attribute) | **PUT** /api/v1/product-attributes/{attribute_id} | 


# **create_product_attribute**
> ProductAttribute create_product_attribute(product_attribute_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.product_attribute import ProductAttribute
from simplebilly_api.models.product_attribute_create import ProductAttributeCreate
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
    api_instance = simplebilly_api.ProductAttributeApi(api_client)
    product_attribute_create = simplebilly_api.ProductAttributeCreate() # ProductAttributeCreate | 

    try:
        api_response = api_instance.create_product_attribute(product_attribute_create)
        print("The response of ProductAttributeApi->create_product_attribute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductAttributeApi->create_product_attribute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_attribute_create** | [**ProductAttributeCreate**](ProductAttributeCreate.md)|  | 

### Return type

[**ProductAttribute**](ProductAttribute.md)

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

# **delete_product_attribute**
> delete_product_attribute(attribute_id)

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
    api_instance = simplebilly_api.ProductAttributeApi(api_client)
    attribute_id = 'attribute_id_example' # str | 

    try:
        api_instance.delete_product_attribute(attribute_id)
    except Exception as e:
        print("Exception when calling ProductAttributeApi->delete_product_attribute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attribute_id** | **str**|  | 

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

# **get_product_attribute**
> ProductAttribute get_product_attribute(attribute_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.product_attribute import ProductAttribute
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
    api_instance = simplebilly_api.ProductAttributeApi(api_client)
    attribute_id = 'attribute_id_example' # str | 

    try:
        api_response = api_instance.get_product_attribute(attribute_id)
        print("The response of ProductAttributeApi->get_product_attribute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductAttributeApi->get_product_attribute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attribute_id** | **str**|  | 

### Return type

[**ProductAttribute**](ProductAttribute.md)

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

# **list_product_attributes**
> List[ProductAttribute] list_product_attributes(page=page, page_size=page_size, product_id=product_id, is_filterable=is_filterable, search=search)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.product_attribute import ProductAttribute
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
    api_instance = simplebilly_api.ProductAttributeApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    is_filterable = True # bool |  (optional)
    search = 'search_example' # str |  (optional)

    try:
        api_response = api_instance.list_product_attributes(page=page, page_size=page_size, product_id=product_id, is_filterable=is_filterable, search=search)
        print("The response of ProductAttributeApi->list_product_attributes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductAttributeApi->list_product_attributes: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **product_id** | **UUID**|  | [optional] 
 **is_filterable** | **bool**|  | [optional] 
 **search** | **str**|  | [optional] 

### Return type

[**List[ProductAttribute]**](ProductAttribute.md)

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

# **update_product_attribute**
> ProductAttribute update_product_attribute(attribute_id, product_attribute_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.product_attribute import ProductAttribute
from simplebilly_api.models.product_attribute_update import ProductAttributeUpdate
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
    api_instance = simplebilly_api.ProductAttributeApi(api_client)
    attribute_id = 'attribute_id_example' # str | 
    product_attribute_update = simplebilly_api.ProductAttributeUpdate() # ProductAttributeUpdate | 

    try:
        api_response = api_instance.update_product_attribute(attribute_id, product_attribute_update)
        print("The response of ProductAttributeApi->update_product_attribute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductAttributeApi->update_product_attribute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attribute_id** | **str**|  | 
 **product_attribute_update** | [**ProductAttributeUpdate**](ProductAttributeUpdate.md)|  | 

### Return type

[**ProductAttribute**](ProductAttribute.md)

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

