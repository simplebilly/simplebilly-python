# simplebilly_api.ShippingThresholdApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_threshold**](ShippingThresholdApi.md#create_shipping_threshold) | **POST** /api/v1/shipping-thresholds | 
[**delete_shipping_threshold**](ShippingThresholdApi.md#delete_shipping_threshold) | **DELETE** /api/v1/shipping-thresholds/{threshold_id} | 
[**get_deliverable**](ShippingThresholdApi.md#get_deliverable) | **GET** /api/v1/shipping-thresholds/deliverable | 
[**get_shipping_threshold**](ShippingThresholdApi.md#get_shipping_threshold) | **GET** /api/v1/shipping-thresholds/{threshold_id} | 
[**list_shipping_thresholds**](ShippingThresholdApi.md#list_shipping_thresholds) | **GET** /api/v1/shipping-thresholds/ | 
[**update_shipping_threshold**](ShippingThresholdApi.md#update_shipping_threshold) | **PUT** /api/v1/shipping-thresholds/{threshold_id} | 


# **create_shipping_threshold**
> ShippingThreshold create_shipping_threshold(shipping_threshold_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.shipping_threshold import ShippingThreshold
from simplebilly_api.models.shipping_threshold_create import ShippingThresholdCreate
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
    api_instance = simplebilly_api.ShippingThresholdApi(api_client)
    shipping_threshold_create = simplebilly_api.ShippingThresholdCreate() # ShippingThresholdCreate | 

    try:
        api_response = api_instance.create_shipping_threshold(shipping_threshold_create)
        print("The response of ShippingThresholdApi->create_shipping_threshold:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShippingThresholdApi->create_shipping_threshold: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipping_threshold_create** | [**ShippingThresholdCreate**](ShippingThresholdCreate.md)|  | 

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

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

# **delete_shipping_threshold**
> delete_shipping_threshold(threshold_id)

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
    api_instance = simplebilly_api.ShippingThresholdApi(api_client)
    threshold_id = 'threshold_id_example' # str | 

    try:
        api_instance.delete_shipping_threshold(threshold_id)
    except Exception as e:
        print("Exception when calling ShippingThresholdApi->delete_shipping_threshold: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **threshold_id** | **str**|  | 

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

# **get_deliverable**
> DeliverableResponse get_deliverable(product_id, warehouse_id=warehouse_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.deliverable_response import DeliverableResponse
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
    api_instance = simplebilly_api.ShippingThresholdApi(api_client)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    warehouse_id = 'warehouse_id_example' # str |  (optional)

    try:
        api_response = api_instance.get_deliverable(product_id, warehouse_id=warehouse_id)
        print("The response of ShippingThresholdApi->get_deliverable:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShippingThresholdApi->get_deliverable: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **product_id** | **UUID**|  | 
 **warehouse_id** | **str**|  | [optional] 

### Return type

[**DeliverableResponse**](DeliverableResponse.md)

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

# **get_shipping_threshold**
> ShippingThreshold get_shipping_threshold(threshold_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.shipping_threshold import ShippingThreshold
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
    api_instance = simplebilly_api.ShippingThresholdApi(api_client)
    threshold_id = 'threshold_id_example' # str | 

    try:
        api_response = api_instance.get_shipping_threshold(threshold_id)
        print("The response of ShippingThresholdApi->get_shipping_threshold:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShippingThresholdApi->get_shipping_threshold: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **threshold_id** | **str**|  | 

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

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

# **list_shipping_thresholds**
> List[ShippingThreshold] list_shipping_thresholds(page=page, page_size=page_size, product_id=product_id, warehouse_id=warehouse_id, is_active=is_active)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.shipping_threshold import ShippingThreshold
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
    api_instance = simplebilly_api.ShippingThresholdApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    warehouse_id = 'warehouse_id_example' # str |  (optional)
    is_active = True # bool |  (optional)

    try:
        api_response = api_instance.list_shipping_thresholds(page=page, page_size=page_size, product_id=product_id, warehouse_id=warehouse_id, is_active=is_active)
        print("The response of ShippingThresholdApi->list_shipping_thresholds:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShippingThresholdApi->list_shipping_thresholds: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **product_id** | **UUID**|  | [optional] 
 **warehouse_id** | **str**|  | [optional] 
 **is_active** | **bool**|  | [optional] 

### Return type

[**List[ShippingThreshold]**](ShippingThreshold.md)

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

# **update_shipping_threshold**
> ShippingThreshold update_shipping_threshold(threshold_id, shipping_threshold_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.shipping_threshold import ShippingThreshold
from simplebilly_api.models.shipping_threshold_update import ShippingThresholdUpdate
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
    api_instance = simplebilly_api.ShippingThresholdApi(api_client)
    threshold_id = 'threshold_id_example' # str | 
    shipping_threshold_update = simplebilly_api.ShippingThresholdUpdate() # ShippingThresholdUpdate | 

    try:
        api_response = api_instance.update_shipping_threshold(threshold_id, shipping_threshold_update)
        print("The response of ShippingThresholdApi->update_shipping_threshold:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShippingThresholdApi->update_shipping_threshold: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **threshold_id** | **str**|  | 
 **shipping_threshold_update** | [**ShippingThresholdUpdate**](ShippingThresholdUpdate.md)|  | 

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

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

