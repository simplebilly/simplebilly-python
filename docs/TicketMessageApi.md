# simplebilly_api.TicketMessageApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_messages_api**](TicketMessageApi.md#list_messages_api) | **GET** /api/v1/support/tickets/{ticket_id}/messages | 
[**send_message_api**](TicketMessageApi.md#send_message_api) | **POST** /api/v1/support/tickets/{ticket_id}/messages | 


# **list_messages_api**
> List[TicketMessage] list_messages_api(ticket_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.ticket_message import TicketMessage
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
    api_instance = simplebilly_api.TicketMessageApi(api_client)
    ticket_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_response = api_instance.list_messages_api(ticket_id)
        print("The response of TicketMessageApi->list_messages_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TicketMessageApi->list_messages_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticket_id** | **UUID**|  | 

### Return type

[**List[TicketMessage]**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Messages for a ticket |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_message_api**
> TicketMessage send_message_api(ticket_id, send_message_dto)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.send_message_dto import SendMessageDto
from simplebilly_api.models.ticket_message import TicketMessage
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
    api_instance = simplebilly_api.TicketMessageApi(api_client)
    ticket_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    send_message_dto = simplebilly_api.SendMessageDto() # SendMessageDto | 

    try:
        api_response = api_instance.send_message_api(ticket_id, send_message_dto)
        print("The response of TicketMessageApi->send_message_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TicketMessageApi->send_message_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticket_id** | **UUID**|  | 
 **send_message_dto** | [**SendMessageDto**](SendMessageDto.md)|  | 

### Return type

[**TicketMessage**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Message sent |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

