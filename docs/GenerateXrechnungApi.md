# simplebilly_api.GenerateXrechnungApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generate_xrechnung_api**](GenerateXrechnungApi.md#generate_xrechnung_api) | **GET** /api/v1/invoices/{id}/xrechnung | 


# **generate_xrechnung_api**
> XRechnungResponse generate_xrechnung_api(id, supplier_name=supplier_name, supplier_street=supplier_street, supplier_city=supplier_city, supplier_zip=supplier_zip, supplier_country=supplier_country, supplier_vat_id=supplier_vat_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.x_rechnung_response import XRechnungResponse
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
    api_instance = simplebilly_api.GenerateXrechnungApi(api_client)
    id = 'id_example' # str | 
    supplier_name = 'supplier_name_example' # str |  (optional)
    supplier_street = 'supplier_street_example' # str |  (optional)
    supplier_city = 'supplier_city_example' # str |  (optional)
    supplier_zip = 'supplier_zip_example' # str |  (optional)
    supplier_country = 'supplier_country_example' # str |  (optional)
    supplier_vat_id = 'supplier_vat_id_example' # str |  (optional)

    try:
        api_response = api_instance.generate_xrechnung_api(id, supplier_name=supplier_name, supplier_street=supplier_street, supplier_city=supplier_city, supplier_zip=supplier_zip, supplier_country=supplier_country, supplier_vat_id=supplier_vat_id)
        print("The response of GenerateXrechnungApi->generate_xrechnung_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GenerateXrechnungApi->generate_xrechnung_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **supplier_name** | **str**|  | [optional] 
 **supplier_street** | **str**|  | [optional] 
 **supplier_city** | **str**|  | [optional] 
 **supplier_zip** | **str**|  | [optional] 
 **supplier_country** | **str**|  | [optional] 
 **supplier_vat_id** | **str**|  | [optional] 

### Return type

[**XRechnungResponse**](XRechnungResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | XRechnung XML |  -  |
**404** | Invoice not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

