# simplebilly_api.OnlineshopApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_smtp_config_api**](OnlineshopApi.md#get_smtp_config_api) | **GET** /api/v1/settings/smtp | 
[**save_smtp_config_api**](OnlineshopApi.md#save_smtp_config_api) | **PUT** /api/v1/settings/smtp | 


# **get_smtp_config_api**
> SmtpConfig get_smtp_config_api()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.smtp_config import SmtpConfig
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
    api_instance = simplebilly_api.OnlineshopApi(api_client)

    try:
        api_response = api_instance.get_smtp_config_api()
        print("The response of OnlineshopApi->get_smtp_config_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnlineshopApi->get_smtp_config_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SmtpConfig**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Tenant SMTP config (null if unset) |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **save_smtp_config_api**
> SmtpConfig save_smtp_config_api(smtp_config=smtp_config)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.smtp_config import SmtpConfig
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
    api_instance = simplebilly_api.OnlineshopApi(api_client)
    smtp_config = simplebilly_api.SmtpConfig() # SmtpConfig |  (optional)

    try:
        api_response = api_instance.save_smtp_config_api(smtp_config=smtp_config)
        print("The response of OnlineshopApi->save_smtp_config_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnlineshopApi->save_smtp_config_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **smtp_config** | [**SmtpConfig**](SmtpConfig.md)|  | [optional] 

### Return type

[**SmtpConfig**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Tenant SMTP config saved |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

