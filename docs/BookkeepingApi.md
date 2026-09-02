# simplebilly_api.BookkeepingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allocate_payment_api**](BookkeepingApi.md#allocate_payment_api) | **POST** /api/v1/payments/allocate | Allocate a payment to an invoice
[**bwa_report_api**](BookkeepingApi.md#bwa_report_api) | **GET** /api/v1/bookkeeping/bwa | Get BWA (Betriebswirtschaftliche Auswertung) report
[**elster_status_api**](BookkeepingApi.md#elster_status_api) | **GET** /api/v1/bookkeeping/elster/status | 
[**elster_validate_api**](BookkeepingApi.md#elster_validate_api) | **POST** /api/v1/bookkeeping/ustva/elster-validate | 
[**elster_xml_api**](BookkeepingApi.md#elster_xml_api) | **GET** /api/v1/bookkeeping/ustva/elster-xml | 
[**get_cashflow**](BookkeepingApi.md#get_cashflow) | **GET** /api/v1/bookkeeping/cashflow | GET /api/v1/bookkeeping/cashflow Returns operating, investing, and financing cashflow for the given period.
[**get_liquidity**](BookkeepingApi.md#get_liquidity) | **GET** /api/v1/bookkeeping/liquidity | GET /api/v1/bookkeeping/liquidity Returns current liquidity position with ratios.
[**get_open_invoices_api**](BookkeepingApi.md#get_open_invoices_api) | **GET** /api/v1/payments/open-invoices/{customer_id} | Get open invoices for a customer
[**get_verfahrensdokumentation**](BookkeepingApi.md#get_verfahrensdokumentation) | **GET** /api/v1/bookkeeping/verfahrensdokumentation | GET /api/v1/bookkeeping/verfahrensdokumentation Returns the complete compliance catalog of all documented modules.
[**run_dunning_api**](BookkeepingApi.md#run_dunning_api) | **POST** /api/v1/bookkeeping/dunning | 


# **allocate_payment_api**
> allocate_payment_api(allocate_payment_request)

Allocate a payment to an invoice

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.allocate_payment_request import AllocatePaymentRequest
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
    api_instance = simplebilly_api.BookkeepingApi(api_client)
    allocate_payment_request = simplebilly_api.AllocatePaymentRequest() # AllocatePaymentRequest | 

    try:
        # Allocate a payment to an invoice
        api_instance.allocate_payment_api(allocate_payment_request)
    except Exception as e:
        print("Exception when calling BookkeepingApi->allocate_payment_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **allocate_payment_request** | [**AllocatePaymentRequest**](AllocatePaymentRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Payment allocated successfully |  -  |
**400** | Invalid request |  -  |
**404** | Payment or invoice not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **bwa_report_api**
> BWAReport bwa_report_api(year=year, month=month)

Get BWA (Betriebswirtschaftliche Auswertung) report

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.bwa_report import BWAReport
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
    api_instance = simplebilly_api.BookkeepingApi(api_client)
    year = 56 # int |  (optional)
    month = 56 # int |  (optional)

    try:
        # Get BWA (Betriebswirtschaftliche Auswertung) report
        api_response = api_instance.bwa_report_api(year=year, month=month)
        print("The response of BookkeepingApi->bwa_report_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BookkeepingApi->bwa_report_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**|  | [optional] 
 **month** | **int**|  | [optional] 

### Return type

[**BWAReport**](BWAReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | BWA Report |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **elster_status_api**
> ElsterStatus elster_status_api()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.elster_status import ElsterStatus
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
    api_instance = simplebilly_api.BookkeepingApi(api_client)

    try:
        api_response = api_instance.elster_status_api()
        print("The response of BookkeepingApi->elster_status_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BookkeepingApi->elster_status_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ElsterStatus**](ElsterStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | ELSTER integration status |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **elster_validate_api**
> elster_validate_api(zeitraum)

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
    api_instance = simplebilly_api.BookkeepingApi(api_client)
    zeitraum = 'zeitraum_example' # str | 

    try:
        api_instance.elster_validate_api(zeitraum)
    except Exception as e:
        print("Exception when calling BookkeepingApi->elster_validate_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **zeitraum** | **str**|  | 

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
**200** | Validate UStVA XML (mock or ERiC) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **elster_xml_api**
> elster_xml_api(zeitraum)

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
    api_instance = simplebilly_api.BookkeepingApi(api_client)
    zeitraum = 'zeitraum_example' # str | 

    try:
        api_instance.elster_xml_api(zeitraum)
    except Exception as e:
        print("Exception when calling BookkeepingApi->elster_xml_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **zeitraum** | **str**|  | 

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
**200** | ELSTER UStVA XML template (manual upload) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_cashflow**
> CashflowReport get_cashflow(year=year, month=month)

GET /api/v1/bookkeeping/cashflow Returns operating, investing, and financing cashflow for the given period.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.cashflow_report import CashflowReport
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
    api_instance = simplebilly_api.BookkeepingApi(api_client)
    year = 56 # int |  (optional)
    month = 56 # int |  (optional)

    try:
        # GET /api/v1/bookkeeping/cashflow Returns operating, investing, and financing cashflow for the given period.
        api_response = api_instance.get_cashflow(year=year, month=month)
        print("The response of BookkeepingApi->get_cashflow:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BookkeepingApi->get_cashflow: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**|  | [optional] 
 **month** | **int**|  | [optional] 

### Return type

[**CashflowReport**](CashflowReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Cashflow report |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_liquidity**
> LiquidityPosition get_liquidity()

GET /api/v1/bookkeeping/liquidity Returns current liquidity position with ratios.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.liquidity_position import LiquidityPosition
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
    api_instance = simplebilly_api.BookkeepingApi(api_client)

    try:
        # GET /api/v1/bookkeeping/liquidity Returns current liquidity position with ratios.
        api_response = api_instance.get_liquidity()
        print("The response of BookkeepingApi->get_liquidity:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BookkeepingApi->get_liquidity: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**LiquidityPosition**](LiquidityPosition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Liquidity position |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_open_invoices_api**
> List[Invoice] get_open_invoices_api(customer_id)

Get open invoices for a customer

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.invoice import Invoice
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
    api_instance = simplebilly_api.BookkeepingApi(api_client)
    customer_id = 'customer_id_example' # str | 

    try:
        # Get open invoices for a customer
        api_response = api_instance.get_open_invoices_api(customer_id)
        print("The response of BookkeepingApi->get_open_invoices_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BookkeepingApi->get_open_invoices_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_id** | **str**|  | 

### Return type

[**List[Invoice]**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Open invoices list |  -  |
**404** | Customer not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_verfahrensdokumentation**
> Verfahrensdokumentation get_verfahrensdokumentation()

GET /api/v1/bookkeeping/verfahrensdokumentation Returns the complete compliance catalog of all documented modules.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.verfahrensdokumentation import Verfahrensdokumentation
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
    api_instance = simplebilly_api.BookkeepingApi(api_client)

    try:
        # GET /api/v1/bookkeeping/verfahrensdokumentation Returns the complete compliance catalog of all documented modules.
        api_response = api_instance.get_verfahrensdokumentation()
        print("The response of BookkeepingApi->get_verfahrensdokumentation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BookkeepingApi->get_verfahrensdokumentation: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Verfahrensdokumentation**](Verfahrensdokumentation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Verfahrensdokumentation |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **run_dunning_api**
> DunningResult run_dunning_api()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.dunning_result import DunningResult
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
    api_instance = simplebilly_api.BookkeepingApi(api_client)

    try:
        api_response = api_instance.run_dunning_api()
        print("The response of BookkeepingApi->run_dunning_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BookkeepingApi->run_dunning_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**DunningResult**](DunningResult.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Dunning run completed successfully |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

