# simplebilly_api.PublicReturnsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_public_return_status**](PublicReturnsApi.md#get_public_return_status) | **GET** /api/v1/public/returns/status | Customer checks the status of a return (public, no auth). The return is only revealed when its linked order&#39;s email matches.
[**list_public_returns**](PublicReturnsApi.md#list_public_returns) | **GET** /api/v1/public/returns/list | List all returns for an order (public, no auth).
[**request_public_return**](PublicReturnsApi.md#request_public_return) | **POST** /api/v1/public/returns/request | Customer requests a return for an order (public, no auth).


# **get_public_return_status**
> PublicReturnStatusResponse get_public_return_status(email, return_number=return_number, return_order_id=return_order_id, order_number=order_number)

Customer checks the status of a return (public, no auth). The return is only revealed when its linked order's email matches.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.public_return_status_response import PublicReturnStatusResponse
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
    api_instance = simplebilly_api.PublicReturnsApi(api_client)
    email = 'email_example' # str | 
    return_number = 'return_number_example' # str | Either return_number or return_order_id must be provided. (optional)
    return_order_id = 'return_order_id_example' # str |  (optional)
    order_number = 'order_number_example' # str |  (optional)

    try:
        # Customer checks the status of a return (public, no auth). The return is only revealed when its linked order's email matches.
        api_response = api_instance.get_public_return_status(email, return_number=return_number, return_order_id=return_order_id, order_number=order_number)
        print("The response of PublicReturnsApi->get_public_return_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicReturnsApi->get_public_return_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **str**|  | 
 **return_number** | **str**| Either return_number or return_order_id must be provided. | [optional] 
 **return_order_id** | **str**|  | [optional] 
 **order_number** | **str**|  | [optional] 

### Return type

[**PublicReturnStatusResponse**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Return status |  -  |
**400** | Bad request (missing return identifier) |  -  |
**404** | Return not found or email mismatch |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_public_returns**
> List[PublicReturnStatusResponse] list_public_returns(order_number, email)

List all returns for an order (public, no auth).

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.public_return_status_response import PublicReturnStatusResponse
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
    api_instance = simplebilly_api.PublicReturnsApi(api_client)
    order_number = 'order_number_example' # str | 
    email = 'email_example' # str | 

    try:
        # List all returns for an order (public, no auth).
        api_response = api_instance.list_public_returns(order_number, email)
        print("The response of PublicReturnsApi->list_public_returns:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicReturnsApi->list_public_returns: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_number** | **str**|  | 
 **email** | **str**|  | 

### Return type

[**List[PublicReturnStatusResponse]**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Returns for the order |  -  |
**404** | Order not found or email mismatch |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **request_public_return**
> PublicReturnResponse request_public_return(public_return_request)

Customer requests a return for an order (public, no auth).

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.public_return_request import PublicReturnRequest
from simplebilly_api.models.public_return_response import PublicReturnResponse
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
    api_instance = simplebilly_api.PublicReturnsApi(api_client)
    public_return_request = simplebilly_api.PublicReturnRequest() # PublicReturnRequest | 

    try:
        # Customer requests a return for an order (public, no auth).
        api_response = api_instance.request_public_return(public_return_request)
        print("The response of PublicReturnsApi->request_public_return:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicReturnsApi->request_public_return: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **public_return_request** | [**PublicReturnRequest**](PublicReturnRequest.md)|  | 

### Return type

[**PublicReturnResponse**](PublicReturnResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Return requested |  -  |
**400** | Bad request (item not in order / quantity too high) |  -  |
**404** | Order not found or email mismatch |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

