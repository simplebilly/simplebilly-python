# simplebilly_api.InstituteApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**institute_status_api**](InstituteApi.md#institute_status_api) | **GET** /api/v1/bookkeeping/institute/status | 


# **institute_status_api**
> InstituteStatus institute_status_api()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.institute_status import InstituteStatus
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
    api_instance = simplebilly_api.InstituteApi(api_client)

    try:
        api_response = api_instance.institute_status_api()
        print("The response of InstituteApi->institute_status_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstituteApi->institute_status_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**InstituteStatus**](InstituteStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Institut-Status: Fristen und Checkliste (KWG § 26, HGB § 340k/§ 341k, HGB § 325, GwG § 8) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

