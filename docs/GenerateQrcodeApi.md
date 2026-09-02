# simplebilly_api.GenerateQrcodeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generate_qrcode_api**](GenerateQrcodeApi.md#generate_qrcode_api) | **GET** /api/v1/invoices/{id}/qrcode | 


# **generate_qrcode_api**
> QRCodeResponse generate_qrcode_api(iban, id, holder_name=holder_name, bic=bic, amount=amount, reference=reference, purpose=purpose)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.qr_code_response import QRCodeResponse
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
    api_instance = simplebilly_api.GenerateQrcodeApi(api_client)
    iban = 'iban_example' # str | 
    id = 'id_example' # str | 
    holder_name = 'holder_name_example' # str |  (optional)
    bic = 'bic_example' # str |  (optional)
    amount = 'amount_example' # str |  (optional)
    reference = 'reference_example' # str |  (optional)
    purpose = 'purpose_example' # str |  (optional)

    try:
        api_response = api_instance.generate_qrcode_api(iban, id, holder_name=holder_name, bic=bic, amount=amount, reference=reference, purpose=purpose)
        print("The response of GenerateQrcodeApi->generate_qrcode_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GenerateQrcodeApi->generate_qrcode_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **iban** | **str**|  | 
 **id** | **str**|  | 
 **holder_name** | **str**|  | [optional] 
 **bic** | **str**|  | [optional] 
 **amount** | **str**|  | [optional] 
 **reference** | **str**|  | [optional] 
 **purpose** | **str**|  | [optional] 

### Return type

[**QRCodeResponse**](QRCodeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | QR Code for invoice payment |  -  |
**404** | Invoice not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

