# simplebilly_api.TenantSettingsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_tenant_settings**](TenantSettingsApi.md#get_tenant_settings) | **GET** /api/v1/settings/tenant | 
[**update_tenant_settings**](TenantSettingsApi.md#update_tenant_settings) | **PUT** /api/v1/settings/tenant | 


# **get_tenant_settings**
> TenantSettings get_tenant_settings()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.tenant_settings import TenantSettings
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
    api_instance = simplebilly_api.TenantSettingsApi(api_client)

    try:
        api_response = api_instance.get_tenant_settings()
        print("The response of TenantSettingsApi->get_tenant_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantSettingsApi->get_tenant_settings: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**TenantSettings**](TenantSettings.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Tenant settings |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_tenant_settings**
> TenantSettings update_tenant_settings(update_tenant_settings)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.tenant_settings import TenantSettings
from simplebilly_api.models.update_tenant_settings import UpdateTenantSettings
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
    api_instance = simplebilly_api.TenantSettingsApi(api_client)
    update_tenant_settings = simplebilly_api.UpdateTenantSettings() # UpdateTenantSettings | 

    try:
        api_response = api_instance.update_tenant_settings(update_tenant_settings)
        print("The response of TenantSettingsApi->update_tenant_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TenantSettingsApi->update_tenant_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **update_tenant_settings** | [**UpdateTenantSettings**](UpdateTenantSettings.md)|  | 

### Return type

[**TenantSettings**](TenantSettings.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated tenant settings |  -  |
**400** | Bad request |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

