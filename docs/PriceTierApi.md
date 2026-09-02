# simplebilly_api.PriceTierApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_price_tier**](PriceTierApi.md#create_price_tier) | **POST** /api/v1/price-tiers | 
[**delete_price_tier**](PriceTierApi.md#delete_price_tier) | **DELETE** /api/v1/price-tiers/{price_tier_id} | 
[**get_price_tier**](PriceTierApi.md#get_price_tier) | **GET** /api/v1/price-tiers/{price_tier_id} | 
[**get_resolved_price**](PriceTierApi.md#get_resolved_price) | **GET** /api/v1/price-tiers/resolved | 
[**list_price_tiers**](PriceTierApi.md#list_price_tiers) | **GET** /api/v1/price-tiers/ | 
[**update_price_tier**](PriceTierApi.md#update_price_tier) | **PUT** /api/v1/price-tiers/{price_tier_id} | 


# **create_price_tier**
> PriceTier create_price_tier(price_tier_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.price_tier import PriceTier
from simplebilly_api.models.price_tier_create import PriceTierCreate
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
    api_instance = simplebilly_api.PriceTierApi(api_client)
    price_tier_create = simplebilly_api.PriceTierCreate() # PriceTierCreate | 

    try:
        api_response = api_instance.create_price_tier(price_tier_create)
        print("The response of PriceTierApi->create_price_tier:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PriceTierApi->create_price_tier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **price_tier_create** | [**PriceTierCreate**](PriceTierCreate.md)|  | 

### Return type

[**PriceTier**](PriceTier.md)

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

# **delete_price_tier**
> delete_price_tier(price_tier_id)

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
    api_instance = simplebilly_api.PriceTierApi(api_client)
    price_tier_id = 'price_tier_id_example' # str | 

    try:
        api_instance.delete_price_tier(price_tier_id)
    except Exception as e:
        print("Exception when calling PriceTierApi->delete_price_tier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **price_tier_id** | **str**|  | 

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

# **get_price_tier**
> PriceTier get_price_tier(price_tier_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.price_tier import PriceTier
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
    api_instance = simplebilly_api.PriceTierApi(api_client)
    price_tier_id = 'price_tier_id_example' # str | 

    try:
        api_response = api_instance.get_price_tier(price_tier_id)
        print("The response of PriceTierApi->get_price_tier:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PriceTierApi->get_price_tier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **price_tier_id** | **str**|  | 

### Return type

[**PriceTier**](PriceTier.md)

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

# **get_resolved_price**
> ResolvedPriceResponse get_resolved_price(product_id, quantity=quantity, contact_id=contact_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.resolved_price_response import ResolvedPriceResponse
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
    api_instance = simplebilly_api.PriceTierApi(api_client)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    quantity = 56 # int |  (optional)
    contact_id = 'contact_id_example' # str | Contact used to match customer-group-scoped tiers. (optional)

    try:
        api_response = api_instance.get_resolved_price(product_id, quantity=quantity, contact_id=contact_id)
        print("The response of PriceTierApi->get_resolved_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PriceTierApi->get_resolved_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_id** | **UUID**|  | 
 **quantity** | **int**|  | [optional] 
 **contact_id** | **str**| Contact used to match customer-group-scoped tiers. | [optional] 

### Return type

[**ResolvedPriceResponse**](ResolvedPriceResponse.md)

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

# **list_price_tiers**
> List[PriceTier] list_price_tiers(page=page, page_size=page_size, product_id=product_id, customer_group_id=customer_group_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.price_tier import PriceTier
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
    api_instance = simplebilly_api.PriceTierApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    customer_group_id = 'customer_group_id_example' # str |  (optional)

    try:
        api_response = api_instance.list_price_tiers(page=page, page_size=page_size, product_id=product_id, customer_group_id=customer_group_id)
        print("The response of PriceTierApi->list_price_tiers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PriceTierApi->list_price_tiers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **product_id** | **UUID**|  | [optional] 
 **customer_group_id** | **str**|  | [optional] 

### Return type

[**List[PriceTier]**](PriceTier.md)

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

# **update_price_tier**
> PriceTier update_price_tier(price_tier_id, price_tier_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.price_tier import PriceTier
from simplebilly_api.models.price_tier_update import PriceTierUpdate
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
    api_instance = simplebilly_api.PriceTierApi(api_client)
    price_tier_id = 'price_tier_id_example' # str | 
    price_tier_update = simplebilly_api.PriceTierUpdate() # PriceTierUpdate | 

    try:
        api_response = api_instance.update_price_tier(price_tier_id, price_tier_update)
        print("The response of PriceTierApi->update_price_tier:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PriceTierApi->update_price_tier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **price_tier_id** | **str**|  | 
 **price_tier_update** | [**PriceTierUpdate**](PriceTierUpdate.md)|  | 

### Return type

[**PriceTier**](PriceTier.md)

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

