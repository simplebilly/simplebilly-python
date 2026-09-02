# simplebilly_api.GoodsReceiptApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_goods_receipt**](GoodsReceiptApi.md#create_goods_receipt) | **POST** /api/v1/goods-receipts | 
[**delete_goods_receipt**](GoodsReceiptApi.md#delete_goods_receipt) | **DELETE** /api/v1/goods-receipts/{goods_receipt_id} | 
[**get_goods_receipt**](GoodsReceiptApi.md#get_goods_receipt) | **GET** /api/v1/goods-receipts/{goods_receipt_id} | 
[**list_goods_receipts**](GoodsReceiptApi.md#list_goods_receipts) | **GET** /api/v1/goods-receipts/ | 


# **create_goods_receipt**
> GoodsReceipt create_goods_receipt(goods_receipt)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.goods_receipt import GoodsReceipt
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
    api_instance = simplebilly_api.GoodsReceiptApi(api_client)
    goods_receipt = simplebilly_api.GoodsReceipt() # GoodsReceipt | 

    try:
        api_response = api_instance.create_goods_receipt(goods_receipt)
        print("The response of GoodsReceiptApi->create_goods_receipt:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GoodsReceiptApi->create_goods_receipt: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **goods_receipt** | [**GoodsReceipt**](GoodsReceipt.md)|  | 

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

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

# **delete_goods_receipt**
> delete_goods_receipt(goods_receipt_id)

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
    api_instance = simplebilly_api.GoodsReceiptApi(api_client)
    goods_receipt_id = 'goods_receipt_id_example' # str | 

    try:
        api_instance.delete_goods_receipt(goods_receipt_id)
    except Exception as e:
        print("Exception when calling GoodsReceiptApi->delete_goods_receipt: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **goods_receipt_id** | **str**|  | 

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

# **get_goods_receipt**
> GoodsReceipt get_goods_receipt(goods_receipt_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.goods_receipt import GoodsReceipt
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
    api_instance = simplebilly_api.GoodsReceiptApi(api_client)
    goods_receipt_id = 'goods_receipt_id_example' # str | 

    try:
        api_response = api_instance.get_goods_receipt(goods_receipt_id)
        print("The response of GoodsReceiptApi->get_goods_receipt:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GoodsReceiptApi->get_goods_receipt: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **goods_receipt_id** | **str**|  | 

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

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

# **list_goods_receipts**
> List[GoodsReceipt] list_goods_receipts(page=page, page_size=page_size, purchase_order_id=purchase_order_id, supplier_name=supplier_name, warehouse_id=warehouse_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.goods_receipt import GoodsReceipt
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
    api_instance = simplebilly_api.GoodsReceiptApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    purchase_order_id = 'purchase_order_id_example' # str |  (optional)
    supplier_name = 'supplier_name_example' # str |  (optional)
    warehouse_id = 'warehouse_id_example' # str |  (optional)

    try:
        api_response = api_instance.list_goods_receipts(page=page, page_size=page_size, purchase_order_id=purchase_order_id, supplier_name=supplier_name, warehouse_id=warehouse_id)
        print("The response of GoodsReceiptApi->list_goods_receipts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GoodsReceiptApi->list_goods_receipts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **purchase_order_id** | **str**|  | [optional] 
 **supplier_name** | **str**|  | [optional] 
 **warehouse_id** | **str**|  | [optional] 

### Return type

[**List[GoodsReceipt]**](GoodsReceipt.md)

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

