# simplebilly_api.PurchaseOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_purchase_order**](PurchaseOrderApi.md#create_purchase_order) | **POST** /api/v1/purchase-orders | 
[**delete_purchase_order**](PurchaseOrderApi.md#delete_purchase_order) | **DELETE** /api/v1/purchase-orders/{purchase_order_id} | 
[**get_purchase_order**](PurchaseOrderApi.md#get_purchase_order) | **GET** /api/v1/purchase-orders/{purchase_order_id} | 
[**list_purchase_orders**](PurchaseOrderApi.md#list_purchase_orders) | **GET** /api/v1/purchase-orders/ | 
[**match_invoice**](PurchaseOrderApi.md#match_invoice) | **POST** /api/v1/purchase-orders/{purchase_order_id}/match-invoice | 3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.
[**update_purchase_order**](PurchaseOrderApi.md#update_purchase_order) | **PUT** /api/v1/purchase-orders/{purchase_order_id} | 
[**update_purchase_order_status**](PurchaseOrderApi.md#update_purchase_order_status) | **PUT** /api/v1/purchase-orders/{purchase_order_id}/status | 


# **create_purchase_order**
> PurchaseOrder create_purchase_order(purchase_order)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.purchase_order import PurchaseOrder
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
    api_instance = simplebilly_api.PurchaseOrderApi(api_client)
    purchase_order = simplebilly_api.PurchaseOrder() # PurchaseOrder | 

    try:
        api_response = api_instance.create_purchase_order(purchase_order)
        print("The response of PurchaseOrderApi->create_purchase_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PurchaseOrderApi->create_purchase_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchase_order** | [**PurchaseOrder**](PurchaseOrder.md)|  | 

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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

# **delete_purchase_order**
> delete_purchase_order(purchase_order_id)

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
    api_instance = simplebilly_api.PurchaseOrderApi(api_client)
    purchase_order_id = 'purchase_order_id_example' # str | 

    try:
        api_instance.delete_purchase_order(purchase_order_id)
    except Exception as e:
        print("Exception when calling PurchaseOrderApi->delete_purchase_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchase_order_id** | **str**|  | 

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

# **get_purchase_order**
> PurchaseOrder get_purchase_order(purchase_order_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.purchase_order import PurchaseOrder
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
    api_instance = simplebilly_api.PurchaseOrderApi(api_client)
    purchase_order_id = 'purchase_order_id_example' # str | 

    try:
        api_response = api_instance.get_purchase_order(purchase_order_id)
        print("The response of PurchaseOrderApi->get_purchase_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PurchaseOrderApi->get_purchase_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchase_order_id** | **str**|  | 

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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

# **list_purchase_orders**
> List[PurchaseOrder] list_purchase_orders(page=page, page_size=page_size, status=status, supplier_name=supplier_name, search=search)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.purchase_order import PurchaseOrder
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
    api_instance = simplebilly_api.PurchaseOrderApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    status = 'status_example' # str |  (optional)
    supplier_name = 'supplier_name_example' # str |  (optional)
    search = 'search_example' # str |  (optional)

    try:
        api_response = api_instance.list_purchase_orders(page=page, page_size=page_size, status=status, supplier_name=supplier_name, search=search)
        print("The response of PurchaseOrderApi->list_purchase_orders:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PurchaseOrderApi->list_purchase_orders: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **status** | **str**|  | [optional] 
 **supplier_name** | **str**|  | [optional] 
 **search** | **str**|  | [optional] 

### Return type

[**List[PurchaseOrder]**](PurchaseOrder.md)

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

# **match_invoice**
> object match_invoice(purchase_order_id, invoice_match_request)

3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.invoice_match_request import InvoiceMatchRequest
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
    api_instance = simplebilly_api.PurchaseOrderApi(api_client)
    purchase_order_id = 'purchase_order_id_example' # str | 
    invoice_match_request = simplebilly_api.InvoiceMatchRequest() # InvoiceMatchRequest | 

    try:
        # 3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.
        api_response = api_instance.match_invoice(purchase_order_id, invoice_match_request)
        print("The response of PurchaseOrderApi->match_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PurchaseOrderApi->match_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchase_order_id** | **str**|  | 
 **invoice_match_request** | [**InvoiceMatchRequest**](InvoiceMatchRequest.md)|  | 

### Return type

**object**

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

# **update_purchase_order**
> PurchaseOrder update_purchase_order(purchase_order_id, body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.purchase_order import PurchaseOrder
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
    api_instance = simplebilly_api.PurchaseOrderApi(api_client)
    purchase_order_id = 'purchase_order_id_example' # str | 
    body = None # object | 

    try:
        api_response = api_instance.update_purchase_order(purchase_order_id, body)
        print("The response of PurchaseOrderApi->update_purchase_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PurchaseOrderApi->update_purchase_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchase_order_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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

# **update_purchase_order_status**
> PurchaseOrder update_purchase_order_status(purchase_order_id, purchase_order_status_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.purchase_order import PurchaseOrder
from simplebilly_api.models.purchase_order_status_update import PurchaseOrderStatusUpdate
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
    api_instance = simplebilly_api.PurchaseOrderApi(api_client)
    purchase_order_id = 'purchase_order_id_example' # str | 
    purchase_order_status_update = simplebilly_api.PurchaseOrderStatusUpdate() # PurchaseOrderStatusUpdate | 

    try:
        api_response = api_instance.update_purchase_order_status(purchase_order_id, purchase_order_status_update)
        print("The response of PurchaseOrderApi->update_purchase_order_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PurchaseOrderApi->update_purchase_order_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchase_order_id** | **str**|  | 
 **purchase_order_status_update** | [**PurchaseOrderStatusUpdate**](PurchaseOrderStatusUpdate.md)|  | 

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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

