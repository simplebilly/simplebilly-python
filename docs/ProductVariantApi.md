# simplebilly_api.ProductVariantApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_product_variant**](ProductVariantApi.md#create_product_variant) | **POST** /api/v1/product-variants | 
[**delete_product_variant**](ProductVariantApi.md#delete_product_variant) | **DELETE** /api/v1/product-variants/{variant_id} | 
[**generate_product_variants**](ProductVariantApi.md#generate_product_variants) | **POST** /api/v1/product-variants/generate | 
[**get_product_variant**](ProductVariantApi.md#get_product_variant) | **GET** /api/v1/product-variants/{variant_id} | 
[**list_product_variants**](ProductVariantApi.md#list_product_variants) | **GET** /api/v1/product-variants/ | 
[**update_product_variant**](ProductVariantApi.md#update_product_variant) | **PUT** /api/v1/product-variants/{variant_id} | 


# **create_product_variant**
> ProductVariant create_product_variant(product_variant)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.product_variant import ProductVariant
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
    api_instance = simplebilly_api.ProductVariantApi(api_client)
    product_variant = simplebilly_api.ProductVariant() # ProductVariant | 

    try:
        api_response = api_instance.create_product_variant(product_variant)
        print("The response of ProductVariantApi->create_product_variant:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductVariantApi->create_product_variant: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_variant** | [**ProductVariant**](ProductVariant.md)|  | 

### Return type

[**ProductVariant**](ProductVariant.md)

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

# **delete_product_variant**
> delete_product_variant(variant_id)

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
    api_instance = simplebilly_api.ProductVariantApi(api_client)
    variant_id = 'variant_id_example' # str | 

    try:
        api_instance.delete_product_variant(variant_id)
    except Exception as e:
        print("Exception when calling ProductVariantApi->delete_product_variant: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **variant_id** | **str**|  | 

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

# **generate_product_variants**
> List[ProductVariant] generate_product_variants(generate_variants_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.generate_variants_request import GenerateVariantsRequest
from simplebilly_api.models.product_variant import ProductVariant
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
    api_instance = simplebilly_api.ProductVariantApi(api_client)
    generate_variants_request = simplebilly_api.GenerateVariantsRequest() # GenerateVariantsRequest | 

    try:
        api_response = api_instance.generate_product_variants(generate_variants_request)
        print("The response of ProductVariantApi->generate_product_variants:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductVariantApi->generate_product_variants: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **generate_variants_request** | [**GenerateVariantsRequest**](GenerateVariantsRequest.md)|  | 

### Return type

[**List[ProductVariant]**](ProductVariant.md)

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

# **get_product_variant**
> ProductVariant get_product_variant(variant_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.product_variant import ProductVariant
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
    api_instance = simplebilly_api.ProductVariantApi(api_client)
    variant_id = 'variant_id_example' # str | 

    try:
        api_response = api_instance.get_product_variant(variant_id)
        print("The response of ProductVariantApi->get_product_variant:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductVariantApi->get_product_variant: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **variant_id** | **str**|  | 

### Return type

[**ProductVariant**](ProductVariant.md)

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

# **list_product_variants**
> List[ProductVariant] list_product_variants(page=page, page_size=page_size, product_id=product_id, is_active=is_active)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.product_variant import ProductVariant
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
    api_instance = simplebilly_api.ProductVariantApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    is_active = True # bool |  (optional)

    try:
        api_response = api_instance.list_product_variants(page=page, page_size=page_size, product_id=product_id, is_active=is_active)
        print("The response of ProductVariantApi->list_product_variants:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductVariantApi->list_product_variants: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **product_id** | **UUID**|  | [optional] 
 **is_active** | **bool**|  | [optional] 

### Return type

[**List[ProductVariant]**](ProductVariant.md)

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

# **update_product_variant**
> ProductVariant update_product_variant(variant_id, body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.product_variant import ProductVariant
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
    api_instance = simplebilly_api.ProductVariantApi(api_client)
    variant_id = 'variant_id_example' # str | 
    body = None # object | 

    try:
        api_response = api_instance.update_product_variant(variant_id, body)
        print("The response of ProductVariantApi->update_product_variant:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProductVariantApi->update_product_variant: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **variant_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**ProductVariant**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

