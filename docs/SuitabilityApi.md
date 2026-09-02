# simplebilly_api.SuitabilityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**shipping_suitability_api**](SuitabilityApi.md#shipping_suitability_api) | **POST** /api/v1/shipping/suitability | 


# **shipping_suitability_api**
> SuitabilityResult shipping_suitability_api(suitability_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.suitability_request import SuitabilityRequest
from simplebilly_api.models.suitability_result import SuitabilityResult
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
    api_instance = simplebilly_api.SuitabilityApi(api_client)
    suitability_request = simplebilly_api.SuitabilityRequest() # SuitabilityRequest | 

    try:
        api_response = api_instance.shipping_suitability_api(suitability_request)
        print("The response of SuitabilityApi->shipping_suitability_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SuitabilityApi->shipping_suitability_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **suitability_request** | [**SuitabilityRequest**](SuitabilityRequest.md)|  | 

### Return type

[**SuitabilityResult**](SuitabilityResult.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Shipping suitability results |  -  |
**400** | Bad request |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

