# simplebilly_api.PaymentGatewayApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_payment_gateway_api**](PaymentGatewayApi.md#create_payment_gateway_api) | **POST** /api/v1/payment-gateways | 
[**delete_payment_gateway_api**](PaymentGatewayApi.md#delete_payment_gateway_api) | **DELETE** /api/v1/payment-gateways/{gateway_id} | 
[**list_payment_gateways_api**](PaymentGatewayApi.md#list_payment_gateways_api) | **GET** /api/v1/payment-gateways/ | 
[**oauth_authorize_api**](PaymentGatewayApi.md#oauth_authorize_api) | **POST** /api/v1/payment-gateways/oauth/authorize | 
[**oauth_callback_api**](PaymentGatewayApi.md#oauth_callback_api) | **POST** /api/v1/payment-gateways/oauth/callback | 
[**update_payment_gateway_api**](PaymentGatewayApi.md#update_payment_gateway_api) | **PUT** /api/v1/payment-gateways/{gateway_id} | 


# **create_payment_gateway_api**
> PaymentGateway create_payment_gateway_api(body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.payment_gateway import PaymentGateway
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
    api_instance = simplebilly_api.PaymentGatewayApi(api_client)
    body = None # object | 

    try:
        api_response = api_instance.create_payment_gateway_api(body)
        print("The response of PaymentGatewayApi->create_payment_gateway_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentGatewayApi->create_payment_gateway_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | 

### Return type

[**PaymentGateway**](PaymentGateway.md)

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

# **delete_payment_gateway_api**
> delete_payment_gateway_api(gateway_id)

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
    api_instance = simplebilly_api.PaymentGatewayApi(api_client)
    gateway_id = 'gateway_id_example' # str | 

    try:
        api_instance.delete_payment_gateway_api(gateway_id)
    except Exception as e:
        print("Exception when calling PaymentGatewayApi->delete_payment_gateway_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gateway_id** | **str**|  | 

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
**200** | Deleted |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_payment_gateways_api**
> List[PaymentGateway] list_payment_gateways_api()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.payment_gateway import PaymentGateway
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
    api_instance = simplebilly_api.PaymentGatewayApi(api_client)

    try:
        api_response = api_instance.list_payment_gateways_api()
        print("The response of PaymentGatewayApi->list_payment_gateways_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentGatewayApi->list_payment_gateways_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[PaymentGateway]**](PaymentGateway.md)

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

# **oauth_authorize_api**
> GatewayOAuthAuthorizeResponse oauth_authorize_api(gateway_o_auth_authorize_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.gateway_o_auth_authorize_request import GatewayOAuthAuthorizeRequest
from simplebilly_api.models.gateway_o_auth_authorize_response import GatewayOAuthAuthorizeResponse
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
    api_instance = simplebilly_api.PaymentGatewayApi(api_client)
    gateway_o_auth_authorize_request = simplebilly_api.GatewayOAuthAuthorizeRequest() # GatewayOAuthAuthorizeRequest | 

    try:
        api_response = api_instance.oauth_authorize_api(gateway_o_auth_authorize_request)
        print("The response of PaymentGatewayApi->oauth_authorize_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentGatewayApi->oauth_authorize_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gateway_o_auth_authorize_request** | [**GatewayOAuthAuthorizeRequest**](GatewayOAuthAuthorizeRequest.md)|  | 

### Return type

[**GatewayOAuthAuthorizeResponse**](GatewayOAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OAuth authorization URL |  -  |
**400** | Bad request |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **oauth_callback_api**
> PaymentGateway oauth_callback_api(gateway_o_auth_callback_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.gateway_o_auth_callback_request import GatewayOAuthCallbackRequest
from simplebilly_api.models.payment_gateway import PaymentGateway
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
    api_instance = simplebilly_api.PaymentGatewayApi(api_client)
    gateway_o_auth_callback_request = simplebilly_api.GatewayOAuthCallbackRequest() # GatewayOAuthCallbackRequest | 

    try:
        api_response = api_instance.oauth_callback_api(gateway_o_auth_callback_request)
        print("The response of PaymentGatewayApi->oauth_callback_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentGatewayApi->oauth_callback_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gateway_o_auth_callback_request** | [**GatewayOAuthCallbackRequest**](GatewayOAuthCallbackRequest.md)|  | 

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Gateway connected |  -  |
**400** | Bad request |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_payment_gateway_api**
> PaymentGateway update_payment_gateway_api(gateway_id, body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.payment_gateway import PaymentGateway
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
    api_instance = simplebilly_api.PaymentGatewayApi(api_client)
    gateway_id = 'gateway_id_example' # str | 
    body = None # object | 

    try:
        api_response = api_instance.update_payment_gateway_api(gateway_id, body)
        print("The response of PaymentGatewayApi->update_payment_gateway_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentGatewayApi->update_payment_gateway_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gateway_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**PaymentGateway**](PaymentGateway.md)

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

