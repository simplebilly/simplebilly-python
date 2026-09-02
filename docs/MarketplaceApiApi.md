# simplebilly_api.MarketplaceApiApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_connection_api**](MarketplaceApiApi.md#create_connection_api) | **POST** /api/v1/marketplace/connections | Create a new connection (for API-key based platforms)
[**delete_connection_api**](MarketplaceApiApi.md#delete_connection_api) | **DELETE** /api/v1/marketplace/connections/{connection_id} | Soft-delete a connection
[**get_connection_api**](MarketplaceApiApi.md#get_connection_api) | **GET** /api/v1/marketplace/connections/{connection_id} | Get a single connection
[**get_sync_direction_api**](MarketplaceApiApi.md#get_sync_direction_api) | **GET** /api/v1/marketplace/connections/{connection_id}/directions | Get current sync direction configuration for a connection
[**get_sync_logs_api**](MarketplaceApiApi.md#get_sync_logs_api) | **GET** /api/v1/marketplace/connections/{connection_id}/logs | Get sync logs for a connection
[**list_connections_api**](MarketplaceApiApi.md#list_connections_api) | **GET** /api/v1/marketplace/connections | List connections for the current tenant
[**list_platforms_api**](MarketplaceApiApi.md#list_platforms_api) | **GET** /api/v1/marketplace/platforms | List all supported platforms
[**oauth_authorize_api**](MarketplaceApiApi.md#oauth_authorize_api) | **POST** /api/v1/marketplace/oauth/authorize | OAuth: initiate authorization flow
[**oauth_callback_api**](MarketplaceApiApi.md#oauth_callback_api) | **POST** /api/v1/marketplace/oauth/callback | OAuth: handle callback after authorization
[**trigger_sync_api**](MarketplaceApiApi.md#trigger_sync_api) | **POST** /api/v1/marketplace/connections/{connection_id}/sync | Trigger sync for a connection
[**update_connection_api**](MarketplaceApiApi.md#update_connection_api) | **PUT** /api/v1/marketplace/connections/{connection_id} | Update a connection
[**update_sync_direction_api**](MarketplaceApiApi.md#update_sync_direction_api) | **PUT** /api/v1/marketplace/connections/{connection_id}/directions | Update per-entity sync direction configuration for a connection
[**webhook_receiver_api**](MarketplaceApiApi.md#webhook_receiver_api) | **POST** /api/v1/marketplace/webhook/{platform}/{connection_id} | Webhook receiver


# **create_connection_api**
> MarketplaceConnection create_connection_api(create_connection_request)

Create a new connection (for API-key based platforms)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.create_connection_request import CreateConnectionRequest
from simplebilly_api.models.marketplace_connection import MarketplaceConnection
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    create_connection_request = simplebilly_api.CreateConnectionRequest() # CreateConnectionRequest | 

    try:
        # Create a new connection (for API-key based platforms)
        api_response = api_instance.create_connection_api(create_connection_request)
        print("The response of MarketplaceApiApi->create_connection_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->create_connection_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_connection_request** | [**CreateConnectionRequest**](CreateConnectionRequest.md)|  | 

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_connection_api**
> delete_connection_api(connection_id)

Soft-delete a connection

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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    connection_id = 'connection_id_example' # str | 

    try:
        # Soft-delete a connection
        api_instance.delete_connection_api(connection_id)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->delete_connection_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connection_id** | **str**|  | 

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
**204** | Deleted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_connection_api**
> MarketplaceConnection get_connection_api(connection_id)

Get a single connection

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.marketplace_connection import MarketplaceConnection
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    connection_id = 'connection_id_example' # str | 

    try:
        # Get a single connection
        api_response = api_instance.get_connection_api(connection_id)
        print("The response of MarketplaceApiApi->get_connection_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->get_connection_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connection_id** | **str**|  | 

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connection details |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_sync_direction_api**
> get_sync_direction_api(connection_id)

Get current sync direction configuration for a connection

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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    connection_id = 'connection_id_example' # str | 

    try:
        # Get current sync direction configuration for a connection
        api_instance.get_sync_direction_api(connection_id)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->get_sync_direction_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connection_id** | **str**|  | 

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
**200** | Current sync directions |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_sync_logs_api**
> List[SyncLog] get_sync_logs_api(connection_id)

Get sync logs for a connection

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.sync_log import SyncLog
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    connection_id = 'connection_id_example' # str | 

    try:
        # Get sync logs for a connection
        api_response = api_instance.get_sync_logs_api(connection_id)
        print("The response of MarketplaceApiApi->get_sync_logs_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->get_sync_logs_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connection_id** | **str**|  | 

### Return type

[**List[SyncLog]**](SyncLog.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Sync logs |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_connections_api**
> List[MarketplaceConnection] list_connections_api()

List connections for the current tenant

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.marketplace_connection import MarketplaceConnection
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)

    try:
        # List connections for the current tenant
        api_response = api_instance.list_connections_api()
        print("The response of MarketplaceApiApi->list_connections_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->list_connections_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[MarketplaceConnection]**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of connections |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_platforms_api**
> List[PlatformInfo] list_platforms_api()

List all supported platforms

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.platform_info import PlatformInfo
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)

    try:
        # List all supported platforms
        api_response = api_instance.list_platforms_api()
        print("The response of MarketplaceApiApi->list_platforms_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->list_platforms_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[PlatformInfo]**](PlatformInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Supported platforms |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **oauth_authorize_api**
> OAuthAuthorizeResponse oauth_authorize_api(o_auth_authorize_request)

OAuth: initiate authorization flow

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.o_auth_authorize_request import OAuthAuthorizeRequest
from simplebilly_api.models.o_auth_authorize_response import OAuthAuthorizeResponse
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    o_auth_authorize_request = simplebilly_api.OAuthAuthorizeRequest() # OAuthAuthorizeRequest | 

    try:
        # OAuth: initiate authorization flow
        api_response = api_instance.oauth_authorize_api(o_auth_authorize_request)
        print("The response of MarketplaceApiApi->oauth_authorize_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->oauth_authorize_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **o_auth_authorize_request** | [**OAuthAuthorizeRequest**](OAuthAuthorizeRequest.md)|  | 

### Return type

[**OAuthAuthorizeResponse**](OAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Authorization URL |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **oauth_callback_api**
> MarketplaceConnection oauth_callback_api(o_auth_callback_request)

OAuth: handle callback after authorization

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.marketplace_connection import MarketplaceConnection
from simplebilly_api.models.o_auth_callback_request import OAuthCallbackRequest
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    o_auth_callback_request = simplebilly_api.OAuthCallbackRequest() # OAuthCallbackRequest | 

    try:
        # OAuth: handle callback after authorization
        api_response = api_instance.oauth_callback_api(o_auth_callback_request)
        print("The response of MarketplaceApiApi->oauth_callback_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->oauth_callback_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **o_auth_callback_request** | [**OAuthCallbackRequest**](OAuthCallbackRequest.md)|  | 

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connection created/updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **trigger_sync_api**
> SyncSummary trigger_sync_api(connection_id, sync_type=sync_type, direction=direction)

Trigger sync for a connection

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.sync_summary import SyncSummary
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    connection_id = 'connection_id_example' # str | 
    sync_type = 'sync_type_example' # str |  (optional)
    direction = 'direction_example' # str |  (optional)

    try:
        # Trigger sync for a connection
        api_response = api_instance.trigger_sync_api(connection_id, sync_type=sync_type, direction=direction)
        print("The response of MarketplaceApiApi->trigger_sync_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->trigger_sync_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connection_id** | **str**|  | 
 **sync_type** | **str**|  | [optional] 
 **direction** | **str**|  | [optional] 

### Return type

[**SyncSummary**](SyncSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Sync triggered |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_connection_api**
> MarketplaceConnection update_connection_api(connection_id, update_connection_request)

Update a connection

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.marketplace_connection import MarketplaceConnection
from simplebilly_api.models.update_connection_request import UpdateConnectionRequest
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    connection_id = 'connection_id_example' # str | 
    update_connection_request = simplebilly_api.UpdateConnectionRequest() # UpdateConnectionRequest | 

    try:
        # Update a connection
        api_response = api_instance.update_connection_api(connection_id, update_connection_request)
        print("The response of MarketplaceApiApi->update_connection_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->update_connection_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connection_id** | **str**|  | 
 **update_connection_request** | [**UpdateConnectionRequest**](UpdateConnectionRequest.md)|  | 

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_sync_direction_api**
> update_sync_direction_api(connection_id, update_sync_direction_request)

Update per-entity sync direction configuration for a connection

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.update_sync_direction_request import UpdateSyncDirectionRequest
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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    connection_id = 'connection_id_example' # str | 
    update_sync_direction_request = simplebilly_api.UpdateSyncDirectionRequest() # UpdateSyncDirectionRequest | 

    try:
        # Update per-entity sync direction configuration for a connection
        api_instance.update_sync_direction_api(connection_id, update_sync_direction_request)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->update_sync_direction_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connection_id** | **str**|  | 
 **update_sync_direction_request** | [**UpdateSyncDirectionRequest**](UpdateSyncDirectionRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Sync directions updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhook_receiver_api**
> webhook_receiver_api(platform, connection_id)

Webhook receiver

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
    api_instance = simplebilly_api.MarketplaceApiApi(api_client)
    platform = 'platform_example' # str | 
    connection_id = 'connection_id_example' # str | 

    try:
        # Webhook receiver
        api_instance.webhook_receiver_api(platform, connection_id)
    except Exception as e:
        print("Exception when calling MarketplaceApiApi->webhook_receiver_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **platform** | **str**|  | 
 **connection_id** | **str**|  | 

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
**200** | Webhook received |  -  |
**401** | Invalid signature |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

