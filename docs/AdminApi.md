# simplebilly_api.AdminApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**trigger_mirror**](AdminApi.md#trigger_mirror) | **POST** /api/v1/admin/storage/mirror | 


# **trigger_mirror**
> MirrorTriggerResponse trigger_mirror()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.mirror_trigger_response import MirrorTriggerResponse
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
    api_instance = simplebilly_api.AdminApi(api_client)

    try:
        api_response = api_instance.trigger_mirror()
        print("The response of AdminApi->trigger_mirror:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AdminApi->trigger_mirror: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**MirrorTriggerResponse**](MirrorTriggerResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Mirror job queued |  -  |
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

