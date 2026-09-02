# simplebilly_api.BankingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bank_lookup_api**](BankingApi.md#bank_lookup_api) | **GET** /api/v1/bookkeeping/banking/lookup | 
[**bank_transactions_api**](BankingApi.md#bank_transactions_api) | **GET** /api/v1/bookkeeping/banking/transactions | 
[**hebesatz_lookup_api**](BankingApi.md#hebesatz_lookup_api) | **GET** /api/v1/bookkeeping/hebesatz | 


# **bank_lookup_api**
> BankLookup bank_lookup_api(iban)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.bank_lookup import BankLookup
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
    api_instance = simplebilly_api.BankingApi(api_client)
    iban = 'iban_example' # str | 

    try:
        api_response = api_instance.bank_lookup_api(iban)
        print("The response of BankingApi->bank_lookup_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BankingApi->bank_lookup_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **iban** | **str**|  | 

### Return type

[**BankLookup**](BankLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Bank-Lookup Ergebnis |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bank_transactions_api**
> bank_transactions_api()

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
    api_instance = simplebilly_api.BankingApi(api_client)

    try:
        api_instance.bank_transactions_api()
    except Exception as e:
        print("Exception when calling BankingApi->bank_transactions_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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
**200** | Bank-Transaktionen |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **hebesatz_lookup_api**
> List[HebesatzLookup] hebesatz_lookup_api(gemeindeschluessel=gemeindeschluessel, plz=plz, name=name, stichtag=stichtag, country_code=country_code)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.hebesatz_lookup import HebesatzLookup
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
    api_instance = simplebilly_api.BankingApi(api_client)
    gemeindeschluessel = 'gemeindeschluessel_example' # str |  (optional)
    plz = 'plz_example' # str |  (optional)
    name = 'name_example' # str |  (optional)
    stichtag = 'stichtag_example' # str | Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from <= date <= valid_to. (optional)
    country_code = 'country_code_example' # str |  (optional)

    try:
        api_response = api_instance.hebesatz_lookup_api(gemeindeschluessel=gemeindeschluessel, plz=plz, name=name, stichtag=stichtag, country_code=country_code)
        print("The response of BankingApi->hebesatz_lookup_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BankingApi->hebesatz_lookup_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gemeindeschluessel** | **str**|  | [optional] 
 **plz** | **str**|  | [optional] 
 **name** | **str**|  | [optional] 
 **stichtag** | **str**| Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from &lt;&#x3D; date &lt;&#x3D; valid_to. | [optional] 
 **country_code** | **str**|  | [optional] 

### Return type

[**List[HebesatzLookup]**](HebesatzLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Hebesatz Lookup |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

