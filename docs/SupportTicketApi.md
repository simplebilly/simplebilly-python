# simplebilly_api.SupportTicketApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_ticket_api**](SupportTicketApi.md#create_ticket_api) | **POST** /api/v1/support/tickets | 
[**delete_ticket_api**](SupportTicketApi.md#delete_ticket_api) | **DELETE** /api/v1/support/tickets/{ticket_id} | 
[**get_ticket_api**](SupportTicketApi.md#get_ticket_api) | **GET** /api/v1/support/tickets/{ticket_id} | 
[**list_tickets_api**](SupportTicketApi.md#list_tickets_api) | **GET** /api/v1/support/tickets | 
[**update_ticket_api**](SupportTicketApi.md#update_ticket_api) | **PUT** /api/v1/support/tickets/{ticket_id} | 


# **create_ticket_api**
> SupportTicket create_ticket_api(create_ticket_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.create_ticket_request import CreateTicketRequest
from simplebilly_api.models.support_ticket import SupportTicket
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
    api_instance = simplebilly_api.SupportTicketApi(api_client)
    create_ticket_request = simplebilly_api.CreateTicketRequest() # CreateTicketRequest | 

    try:
        api_response = api_instance.create_ticket_api(create_ticket_request)
        print("The response of SupportTicketApi->create_ticket_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupportTicketApi->create_ticket_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_ticket_request** | [**CreateTicketRequest**](CreateTicketRequest.md)|  | 

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Ticket created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_ticket_api**
> delete_ticket_api(ticket_id)

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
    api_instance = simplebilly_api.SupportTicketApi(api_client)
    ticket_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_instance.delete_ticket_api(ticket_id)
    except Exception as e:
        print("Exception when calling SupportTicketApi->delete_ticket_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticket_id** | **UUID**|  | 

### Return type

void (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Ticket deleted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_ticket_api**
> SupportTicket get_ticket_api(ticket_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.support_ticket import SupportTicket
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
    api_instance = simplebilly_api.SupportTicketApi(api_client)
    ticket_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_response = api_instance.get_ticket_api(ticket_id)
        print("The response of SupportTicketApi->get_ticket_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupportTicketApi->get_ticket_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticket_id** | **UUID**|  | 

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Ticket detail |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_tickets_api**
> List[SupportTicket] list_tickets_api(status=status, priority=priority, assigned_to=assigned_to, channel_type=channel_type, customer_id=customer_id, search=search, page=page, page_size=page_size)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.support_ticket import SupportTicket
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
    api_instance = simplebilly_api.SupportTicketApi(api_client)
    status = 'status_example' # str |  (optional)
    priority = 'priority_example' # str |  (optional)
    assigned_to = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    channel_type = 'channel_type_example' # str |  (optional)
    customer_id = 'customer_id_example' # str |  (optional)
    search = 'search_example' # str |  (optional)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)

    try:
        api_response = api_instance.list_tickets_api(status=status, priority=priority, assigned_to=assigned_to, channel_type=channel_type, customer_id=customer_id, search=search, page=page, page_size=page_size)
        print("The response of SupportTicketApi->list_tickets_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupportTicketApi->list_tickets_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **str**|  | [optional] 
 **priority** | **str**|  | [optional] 
 **assigned_to** | **UUID**|  | [optional] 
 **channel_type** | **str**|  | [optional] 
 **customer_id** | **str**|  | [optional] 
 **search** | **str**|  | [optional] 
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 

### Return type

[**List[SupportTicket]**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Tickets list |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_ticket_api**
> SupportTicket update_ticket_api(ticket_id, support_ticket_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.support_ticket import SupportTicket
from simplebilly_api.models.support_ticket_update import SupportTicketUpdate
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
    api_instance = simplebilly_api.SupportTicketApi(api_client)
    ticket_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    support_ticket_update = simplebilly_api.SupportTicketUpdate() # SupportTicketUpdate | 

    try:
        api_response = api_instance.update_ticket_api(ticket_id, support_ticket_update)
        print("The response of SupportTicketApi->update_ticket_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupportTicketApi->update_ticket_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticket_id** | **UUID**|  | 
 **support_ticket_update** | [**SupportTicketUpdate**](SupportTicketUpdate.md)|  | 

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Ticket updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

