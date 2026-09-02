# simplebilly_api.GezApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gez_api**](GezApi.md#gez_api) | **GET** /api/v1/bookkeeping/gez | 


# **gez_api**
> GezReport gez_api(jahr=jahr, betriebsstaetten=betriebsstaetten, kfz=kfz, hotelzimmer=hotelzimmer, beschaefigte=beschaefigte)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.gez_report import GezReport
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
    api_instance = simplebilly_api.GezApi(api_client)
    jahr = 56 # int |  (optional)
    betriebsstaetten = 'betriebsstaetten_example' # str | Liste der Betriebsstätten als JSON, z.B. `[{\"name\":\"Filiale 1\",\"beschaefigte\":12}]`. (optional)
    kfz = 56 # int | Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind). (optional)
    hotelzimmer = 56 # int | Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen. (optional)
    beschaefigte = 56 # int | Gesamtzahl der Beschäftigten (verwendet nur, wenn `betriebsstaetten` fehlt; dann wird eine einzelne Betriebsstätte angenommen). (optional)

    try:
        api_response = api_instance.gez_api(jahr=jahr, betriebsstaetten=betriebsstaetten, kfz=kfz, hotelzimmer=hotelzimmer, beschaefigte=beschaefigte)
        print("The response of GezApi->gez_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GezApi->gez_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **jahr** | **int**|  | [optional] 
 **betriebsstaetten** | **str**| Liste der Betriebsstätten als JSON, z.B. &#x60;[{\&quot;name\&quot;:\&quot;Filiale 1\&quot;,\&quot;beschaefigte\&quot;:12}]&#x60;. | [optional] 
 **kfz** | **int**| Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind). | [optional] 
 **hotelzimmer** | **int**| Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen. | [optional] 
 **beschaefigte** | **int**| Gesamtzahl der Beschäftigten (verwendet nur, wenn &#x60;betriebsstaetten&#x60; fehlt; dann wird eine einzelne Betriebsstätte angenommen). | [optional] 

### Return type

[**GezReport**](GezReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Rundfunkbeitrag (GEZ) Berechnung nach § 5 RBStV |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

