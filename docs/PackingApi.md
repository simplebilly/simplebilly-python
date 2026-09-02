# simplebilly_api.PackingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**complete_packing**](PackingApi.md#complete_packing) | **POST** /api/v1/packing/{order_number}/complete | Mark packing as complete and transition order to shipped
[**get_packing_queue**](PackingApi.md#get_packing_queue) | **GET** /api/v1/packing/queue | Get the packing queue - orders ready for packing
[**print_delivery_note**](PackingApi.md#print_delivery_note) | **POST** /api/v1/packing/{order_number}/print-delivery-note | Print delivery note (Lieferschein) for an order
[**print_label**](PackingApi.md#print_label) | **POST** /api/v1/packing/{order_number}/print-label | Print shipping label for an order
[**record_packing_video**](PackingApi.md#record_packing_video) | **POST** /api/v1/packing/{order_number}/record-video | Record video of packing process


# **complete_packing**
> PackingCompleteResponse complete_packing(order_number, packing_complete_request)

Mark packing as complete and transition order to shipped

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.packing_complete_request import PackingCompleteRequest
from simplebilly_api.models.packing_complete_response import PackingCompleteResponse
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
    api_instance = simplebilly_api.PackingApi(api_client)
    order_number = 'order_number_example' # str | 
    packing_complete_request = simplebilly_api.PackingCompleteRequest() # PackingCompleteRequest | 

    try:
        # Mark packing as complete and transition order to shipped
        api_response = api_instance.complete_packing(order_number, packing_complete_request)
        print("The response of PackingApi->complete_packing:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PackingApi->complete_packing: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_number** | **str**|  | 
 **packing_complete_request** | [**PackingCompleteRequest**](PackingCompleteRequest.md)|  | 

### Return type

[**PackingCompleteResponse**](PackingCompleteResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Packing completed |  -  |
**404** | Order not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_packing_queue**
> PackingQueue get_packing_queue(page=page, page_size=page_size, search=search)

Get the packing queue - orders ready for packing

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.packing_queue import PackingQueue
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
    api_instance = simplebilly_api.PackingApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    search = 'search_example' # str |  (optional)

    try:
        # Get the packing queue - orders ready for packing
        api_response = api_instance.get_packing_queue(page=page, page_size=page_size, search=search)
        print("The response of PackingApi->get_packing_queue:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PackingApi->get_packing_queue: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **search** | **str**|  | [optional] 

### Return type

[**PackingQueue**](PackingQueue.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Packing queue |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **print_delivery_note**
> PrintDeliveryNoteResponse print_delivery_note(order_number)

Print delivery note (Lieferschein) for an order

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.print_delivery_note_response import PrintDeliveryNoteResponse
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
    api_instance = simplebilly_api.PackingApi(api_client)
    order_number = 'order_number_example' # str | 

    try:
        # Print delivery note (Lieferschein) for an order
        api_response = api_instance.print_delivery_note(order_number)
        print("The response of PackingApi->print_delivery_note:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PackingApi->print_delivery_note: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_number** | **str**|  | 

### Return type

[**PrintDeliveryNoteResponse**](PrintDeliveryNoteResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Delivery note printed |  -  |
**404** | Order not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **print_label**
> PrintLabelResponse print_label(order_number)

Print shipping label for an order

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.print_label_response import PrintLabelResponse
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
    api_instance = simplebilly_api.PackingApi(api_client)
    order_number = 'order_number_example' # str | 

    try:
        # Print shipping label for an order
        api_response = api_instance.print_label(order_number)
        print("The response of PackingApi->print_label:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PackingApi->print_label: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_number** | **str**|  | 

### Return type

[**PrintLabelResponse**](PrintLabelResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Label printed |  -  |
**404** | Order not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **record_packing_video**
> PackingVideoResponse record_packing_video(order_number, body)

Record video of packing process

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.packing_video_response import PackingVideoResponse
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
    api_instance = simplebilly_api.PackingApi(api_client)
    order_number = 'order_number_example' # str | 
    body = None # object | 

    try:
        # Record video of packing process
        api_response = api_instance.record_packing_video(order_number, body)
        print("The response of PackingApi->record_packing_video:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PackingApi->record_packing_video: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_number** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**PackingVideoResponse**](PackingVideoResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Video recorded |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

