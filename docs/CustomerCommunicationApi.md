# simplebilly_api.CustomerCommunicationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_communication**](CustomerCommunicationApi.md#create_communication) | **POST** /api/v1/communications | 
[**customercommunication_restore**](CustomerCommunicationApi.md#customercommunication_restore) | **POST** /api/v1/communications/{communication_id}/restore | 
[**delete_communication**](CustomerCommunicationApi.md#delete_communication) | **DELETE** /api/v1/communications/{communication_id} | 
[**get_communication**](CustomerCommunicationApi.md#get_communication) | **GET** /api/v1/communications/{communication_id} | 
[**get_contact_history**](CustomerCommunicationApi.md#get_contact_history) | **GET** /api/v1/contacts/{contact_id}/communications | 
[**list_communications**](CustomerCommunicationApi.md#list_communications) | **GET** /api/v1/communications/ | 
[**update_communication**](CustomerCommunicationApi.md#update_communication) | **PUT** /api/v1/communications/{communication_id} | 


# **create_communication**
> CustomerCommunication create_communication(customer_communication_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer_communication import CustomerCommunication
from simplebilly_api.models.customer_communication_create import CustomerCommunicationCreate
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
    api_instance = simplebilly_api.CustomerCommunicationApi(api_client)
    customer_communication_create = simplebilly_api.CustomerCommunicationCreate() # CustomerCommunicationCreate | 

    try:
        api_response = api_instance.create_communication(customer_communication_create)
        print("The response of CustomerCommunicationApi->create_communication:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerCommunicationApi->create_communication: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_communication_create** | [**CustomerCommunicationCreate**](CustomerCommunicationCreate.md)|  | 

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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

# **customercommunication_restore**
> CustomerCommunication customercommunication_restore(communication_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer_communication import CustomerCommunication
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
    api_instance = simplebilly_api.CustomerCommunicationApi(api_client)
    communication_id = 'communication_id_example' # str | 

    try:
        api_response = api_instance.customercommunication_restore(communication_id)
        print("The response of CustomerCommunicationApi->customercommunication_restore:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerCommunicationApi->customercommunication_restore: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **communication_id** | **str**|  | 

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Restored |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_communication**
> delete_communication(communication_id)

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
    api_instance = simplebilly_api.CustomerCommunicationApi(api_client)
    communication_id = 'communication_id_example' # str | 

    try:
        api_instance.delete_communication(communication_id)
    except Exception as e:
        print("Exception when calling CustomerCommunicationApi->delete_communication: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **communication_id** | **str**|  | 

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

# **get_communication**
> CustomerCommunication get_communication(communication_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer_communication import CustomerCommunication
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
    api_instance = simplebilly_api.CustomerCommunicationApi(api_client)
    communication_id = 'communication_id_example' # str | 

    try:
        api_response = api_instance.get_communication(communication_id)
        print("The response of CustomerCommunicationApi->get_communication:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerCommunicationApi->get_communication: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **communication_id** | **str**|  | 

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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

# **get_contact_history**
> ContactHistoryResponse get_contact_history(contact_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.contact_history_response import ContactHistoryResponse
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
    api_instance = simplebilly_api.CustomerCommunicationApi(api_client)
    contact_id = 'contact_id_example' # str | 

    try:
        api_response = api_instance.get_contact_history(contact_id)
        print("The response of CustomerCommunicationApi->get_contact_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerCommunicationApi->get_contact_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contact_id** | **str**|  | 

### Return type

[**ContactHistoryResponse**](ContactHistoryResponse.md)

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

# **list_communications**
> List[CustomerCommunication] list_communications(page=page, page_size=page_size, contact_id=contact_id, channel=channel, direction=direction, var_from=var_from, to=to)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer_communication import CustomerCommunication
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
    api_instance = simplebilly_api.CustomerCommunicationApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    contact_id = 'contact_id_example' # str | Filter history to a single contact. (optional)
    channel = simplebilly_api.CommunicationChannel() # CommunicationChannel |  (optional)
    direction = simplebilly_api.CommunicationDirection() # CommunicationDirection |  (optional)
    var_from = '2013-10-20' # date | Only include communications after this ISO date (inclusive). (optional)
    to = '2013-10-20' # date | Only include communications before this ISO date (inclusive). (optional)

    try:
        api_response = api_instance.list_communications(page=page, page_size=page_size, contact_id=contact_id, channel=channel, direction=direction, var_from=var_from, to=to)
        print("The response of CustomerCommunicationApi->list_communications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerCommunicationApi->list_communications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **contact_id** | **str**| Filter history to a single contact. | [optional] 
 **channel** | [**CommunicationChannel**](.md)|  | [optional] 
 **direction** | [**CommunicationDirection**](.md)|  | [optional] 
 **var_from** | **date**| Only include communications after this ISO date (inclusive). | [optional] 
 **to** | **date**| Only include communications before this ISO date (inclusive). | [optional] 

### Return type

[**List[CustomerCommunication]**](CustomerCommunication.md)

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

# **update_communication**
> CustomerCommunication update_communication(communication_id, customer_communication_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.customer_communication import CustomerCommunication
from simplebilly_api.models.customer_communication_update import CustomerCommunicationUpdate
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
    api_instance = simplebilly_api.CustomerCommunicationApi(api_client)
    communication_id = 'communication_id_example' # str | 
    customer_communication_update = simplebilly_api.CustomerCommunicationUpdate() # CustomerCommunicationUpdate | 

    try:
        api_response = api_instance.update_communication(communication_id, customer_communication_update)
        print("The response of CustomerCommunicationApi->update_communication:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerCommunicationApi->update_communication: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **communication_id** | **str**|  | 
 **customer_communication_update** | [**CustomerCommunicationUpdate**](CustomerCommunicationUpdate.md)|  | 

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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

