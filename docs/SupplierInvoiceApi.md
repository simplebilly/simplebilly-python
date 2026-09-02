# simplebilly_api.SupplierInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_supplier_invoice**](SupplierInvoiceApi.md#create_supplier_invoice) | **POST** /api/v1/supplier-invoices | 
[**delete_supplier_invoice**](SupplierInvoiceApi.md#delete_supplier_invoice) | **DELETE** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**get_supplier_invoice**](SupplierInvoiceApi.md#get_supplier_invoice) | **GET** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**list_supplier_invoices**](SupplierInvoiceApi.md#list_supplier_invoices) | **GET** /api/v1/supplier-invoices/ | 
[**update_supplier_invoice**](SupplierInvoiceApi.md#update_supplier_invoice) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**update_supplier_invoice_status**](SupplierInvoiceApi.md#update_supplier_invoice_status) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id}/status | 


# **create_supplier_invoice**
> SupplierInvoice create_supplier_invoice(supplier_invoice)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.supplier_invoice import SupplierInvoice
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
    api_instance = simplebilly_api.SupplierInvoiceApi(api_client)
    supplier_invoice = simplebilly_api.SupplierInvoice() # SupplierInvoice | 

    try:
        api_response = api_instance.create_supplier_invoice(supplier_invoice)
        print("The response of SupplierInvoiceApi->create_supplier_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupplierInvoiceApi->create_supplier_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplier_invoice** | [**SupplierInvoice**](SupplierInvoice.md)|  | 

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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

# **delete_supplier_invoice**
> delete_supplier_invoice(supplier_invoice_id)

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
    api_instance = simplebilly_api.SupplierInvoiceApi(api_client)
    supplier_invoice_id = 'supplier_invoice_id_example' # str | 

    try:
        api_instance.delete_supplier_invoice(supplier_invoice_id)
    except Exception as e:
        print("Exception when calling SupplierInvoiceApi->delete_supplier_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplier_invoice_id** | **str**|  | 

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
**400** | Bad request |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_supplier_invoice**
> SupplierInvoice get_supplier_invoice(supplier_invoice_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.supplier_invoice import SupplierInvoice
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
    api_instance = simplebilly_api.SupplierInvoiceApi(api_client)
    supplier_invoice_id = 'supplier_invoice_id_example' # str | 

    try:
        api_response = api_instance.get_supplier_invoice(supplier_invoice_id)
        print("The response of SupplierInvoiceApi->get_supplier_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupplierInvoiceApi->get_supplier_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplier_invoice_id** | **str**|  | 

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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

# **list_supplier_invoices**
> List[SupplierInvoice] list_supplier_invoices(page=page, page_size=page_size, status=status, purchase_order_id=purchase_order_id, supplier_name=supplier_name)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.supplier_invoice import SupplierInvoice
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
    api_instance = simplebilly_api.SupplierInvoiceApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    status = 'status_example' # str |  (optional)
    purchase_order_id = 'purchase_order_id_example' # str |  (optional)
    supplier_name = 'supplier_name_example' # str |  (optional)

    try:
        api_response = api_instance.list_supplier_invoices(page=page, page_size=page_size, status=status, purchase_order_id=purchase_order_id, supplier_name=supplier_name)
        print("The response of SupplierInvoiceApi->list_supplier_invoices:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupplierInvoiceApi->list_supplier_invoices: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **status** | **str**|  | [optional] 
 **purchase_order_id** | **str**|  | [optional] 
 **supplier_name** | **str**|  | [optional] 

### Return type

[**List[SupplierInvoice]**](SupplierInvoice.md)

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

# **update_supplier_invoice**
> SupplierInvoice update_supplier_invoice(supplier_invoice_id, body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.supplier_invoice import SupplierInvoice
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
    api_instance = simplebilly_api.SupplierInvoiceApi(api_client)
    supplier_invoice_id = 'supplier_invoice_id_example' # str | 
    body = None # object | 

    try:
        api_response = api_instance.update_supplier_invoice(supplier_invoice_id, body)
        print("The response of SupplierInvoiceApi->update_supplier_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupplierInvoiceApi->update_supplier_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplier_invoice_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad request |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_supplier_invoice_status**
> SupplierInvoice update_supplier_invoice_status(supplier_invoice_id, supplier_invoice_status_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.supplier_invoice import SupplierInvoice
from simplebilly_api.models.supplier_invoice_status_update import SupplierInvoiceStatusUpdate
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
    api_instance = simplebilly_api.SupplierInvoiceApi(api_client)
    supplier_invoice_id = 'supplier_invoice_id_example' # str | 
    supplier_invoice_status_update = simplebilly_api.SupplierInvoiceStatusUpdate() # SupplierInvoiceStatusUpdate | 

    try:
        api_response = api_instance.update_supplier_invoice_status(supplier_invoice_id, supplier_invoice_status_update)
        print("The response of SupplierInvoiceApi->update_supplier_invoice_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SupplierInvoiceApi->update_supplier_invoice_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplier_invoice_id** | **str**|  | 
 **supplier_invoice_status_update** | [**SupplierInvoiceStatusUpdate**](SupplierInvoiceStatusUpdate.md)|  | 

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad request |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

