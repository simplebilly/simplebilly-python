# simplebilly_api.FristenApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fristen_api**](FristenApi.md#fristen_api) | **GET** /api/v1/bookkeeping/fristen | 


# **fristen_api**
> FristenErgebnis fristen_api(bundesland=bundesland, voranmeldungsrhythmus=voranmeldungsrhythmus, dauerfristverlaengerung=dauerfristverlaengerung, est_aktiv=est_aktiv, gewst_aktiv=gewst_aktiv, monate=monate)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.fristen_ergebnis import FristenErgebnis
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
    api_instance = simplebilly_api.FristenApi(api_client)
    bundesland = 'bundesland_example' # str |  (optional)
    voranmeldungsrhythmus = 'voranmeldungsrhythmus_example' # str |  (optional)
    dauerfristverlaengerung = True # bool |  (optional)
    est_aktiv = True # bool |  (optional)
    gewst_aktiv = True # bool |  (optional)
    monate = 56 # int |  (optional)

    try:
        api_response = api_instance.fristen_api(bundesland=bundesland, voranmeldungsrhythmus=voranmeldungsrhythmus, dauerfristverlaengerung=dauerfristverlaengerung, est_aktiv=est_aktiv, gewst_aktiv=gewst_aktiv, monate=monate)
        print("The response of FristenApi->fristen_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FristenApi->fristen_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bundesland** | **str**|  | [optional] 
 **voranmeldungsrhythmus** | **str**|  | [optional] 
 **dauerfristverlaengerung** | **bool**|  | [optional] 
 **est_aktiv** | **bool**|  | [optional] 
 **gewst_aktiv** | **bool**|  | [optional] 
 **monate** | **int**|  | [optional] 

### Return type

[**FristenErgebnis**](FristenErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Steuerliche Fristen |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

