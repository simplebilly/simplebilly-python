# simplebilly_api.ProformaInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**convert_proforma_to_invoice**](ProformaInvoiceApi.md#convert_proforma_to_invoice) | **POST** /api/v1/proforma-invoices/{proforma_id}/convert | 
[**create_proforma_invoice**](ProformaInvoiceApi.md#create_proforma_invoice) | **POST** /api/v1/proforma-invoices | 
[**delete_proforma_invoice**](ProformaInvoiceApi.md#delete_proforma_invoice) | **DELETE** /api/v1/proforma-invoices/{proforma_id} | 
[**get_proforma_invoice**](ProformaInvoiceApi.md#get_proforma_invoice) | **GET** /api/v1/proforma-invoices/{proforma_id} | 
[**list_proforma_invoices**](ProformaInvoiceApi.md#list_proforma_invoices) | **GET** /api/v1/proforma-invoices/ | 
[**update_proforma_invoice**](ProformaInvoiceApi.md#update_proforma_invoice) | **PUT** /api/v1/proforma-invoices/{proforma_id} | 


# **convert_proforma_to_invoice**
> ConvertResponse convert_proforma_to_invoice(proforma_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.convert_response import ConvertResponse
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
    api_instance = simplebilly_api.ProformaInvoiceApi(api_client)
    proforma_id = 'proforma_id_example' # str | 

    try:
        api_response = api_instance.convert_proforma_to_invoice(proforma_id)
        print("The response of ProformaInvoiceApi->convert_proforma_to_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProformaInvoiceApi->convert_proforma_to_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proforma_id** | **str**|  | 

### Return type

[**ConvertResponse**](ConvertResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad request |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_proforma_invoice**
> ProformaInvoice create_proforma_invoice(proforma_invoice)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.proforma_invoice import ProformaInvoice
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
    api_instance = simplebilly_api.ProformaInvoiceApi(api_client)
    proforma_invoice = simplebilly_api.ProformaInvoice() # ProformaInvoice | 

    try:
        api_response = api_instance.create_proforma_invoice(proforma_invoice)
        print("The response of ProformaInvoiceApi->create_proforma_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProformaInvoiceApi->create_proforma_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proforma_invoice** | [**ProformaInvoice**](ProformaInvoice.md)|  | 

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | Bad request |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_proforma_invoice**
> delete_proforma_invoice(proforma_id)

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
    api_instance = simplebilly_api.ProformaInvoiceApi(api_client)
    proforma_id = 'proforma_id_example' # str | 

    try:
        api_instance.delete_proforma_invoice(proforma_id)
    except Exception as e:
        print("Exception when calling ProformaInvoiceApi->delete_proforma_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proforma_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | No Content |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_proforma_invoice**
> ProformaInvoice get_proforma_invoice(proforma_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.proforma_invoice import ProformaInvoice
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
    api_instance = simplebilly_api.ProformaInvoiceApi(api_client)
    proforma_id = 'proforma_id_example' # str | 

    try:
        api_response = api_instance.get_proforma_invoice(proforma_id)
        print("The response of ProformaInvoiceApi->get_proforma_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProformaInvoiceApi->get_proforma_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proforma_id** | **str**|  | 

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_proforma_invoices**
> List[ProformaInvoice] list_proforma_invoices(page=page, page_size=page_size, status=status, customer_id=customer_id, order_number=order_number)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.proforma_invoice import ProformaInvoice
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
    api_instance = simplebilly_api.ProformaInvoiceApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    status = 'status_example' # str |  (optional)
    customer_id = 'customer_id_example' # str |  (optional)
    order_number = 'order_number_example' # str |  (optional)

    try:
        api_response = api_instance.list_proforma_invoices(page=page, page_size=page_size, status=status, customer_id=customer_id, order_number=order_number)
        print("The response of ProformaInvoiceApi->list_proforma_invoices:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProformaInvoiceApi->list_proforma_invoices: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **status** | **str**|  | [optional] 
 **customer_id** | **str**|  | [optional] 
 **order_number** | **str**|  | [optional] 

### Return type

[**List[ProformaInvoice]**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_proforma_invoice**
> ProformaInvoice update_proforma_invoice(proforma_id, body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.proforma_invoice import ProformaInvoice
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
    api_instance = simplebilly_api.ProformaInvoiceApi(api_client)
    proforma_id = 'proforma_id_example' # str | 
    body = None # object | 

    try:
        api_response = api_instance.update_proforma_invoice(proforma_id, body)
        print("The response of ProformaInvoiceApi->update_proforma_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProformaInvoiceApi->update_proforma_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proforma_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

