# simplebilly_api.WarehouseStockApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_warehouse_stock**](WarehouseStockApi.md#create_warehouse_stock) | **POST** /api/v1/warehouses/{warehouse_id}/stock | 
[**delete_warehouse_stock**](WarehouseStockApi.md#delete_warehouse_stock) | **DELETE** /api/v1/warehouses/{warehouse_id}/stock/{product_id} | 
[**list_warehouse_stock**](WarehouseStockApi.md#list_warehouse_stock) | **GET** /api/v1/warehouses/{warehouse_id}/stock | 
[**update_warehouse_stock**](WarehouseStockApi.md#update_warehouse_stock) | **PUT** /api/v1/warehouses/{warehouse_id}/stock/{product_id} | 


# **create_warehouse_stock**
> WarehouseStock create_warehouse_stock(warehouse_id, stock_adjustment)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.stock_adjustment import StockAdjustment
from simplebilly_api.models.warehouse_stock import WarehouseStock
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
    api_instance = simplebilly_api.WarehouseStockApi(api_client)
    warehouse_id = 'warehouse_id_example' # str | 
    stock_adjustment = simplebilly_api.StockAdjustment() # StockAdjustment | 

    try:
        api_response = api_instance.create_warehouse_stock(warehouse_id, stock_adjustment)
        print("The response of WarehouseStockApi->create_warehouse_stock:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WarehouseStockApi->create_warehouse_stock: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouse_id** | **str**|  | 
 **stock_adjustment** | [**StockAdjustment**](StockAdjustment.md)|  | 

### Return type

[**WarehouseStock**](WarehouseStock.md)

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

# **delete_warehouse_stock**
> delete_warehouse_stock(warehouse_id, product_id)

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
    api_instance = simplebilly_api.WarehouseStockApi(api_client)
    warehouse_id = 'warehouse_id_example' # str | 
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_instance.delete_warehouse_stock(warehouse_id, product_id)
    except Exception as e:
        print("Exception when calling WarehouseStockApi->delete_warehouse_stock: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouse_id** | **str**|  | 
 **product_id** | **UUID**|  | 

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

# **list_warehouse_stock**
> List[WarehouseStock] list_warehouse_stock(warehouse_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.warehouse_stock import WarehouseStock
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
    api_instance = simplebilly_api.WarehouseStockApi(api_client)
    warehouse_id = 'warehouse_id_example' # str | 

    try:
        api_response = api_instance.list_warehouse_stock(warehouse_id)
        print("The response of WarehouseStockApi->list_warehouse_stock:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WarehouseStockApi->list_warehouse_stock: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouse_id** | **str**|  | 

### Return type

[**List[WarehouseStock]**](WarehouseStock.md)

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

# **update_warehouse_stock**
> WarehouseStock update_warehouse_stock(warehouse_id, product_id, stock_adjustment)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.stock_adjustment import StockAdjustment
from simplebilly_api.models.warehouse_stock import WarehouseStock
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
    api_instance = simplebilly_api.WarehouseStockApi(api_client)
    warehouse_id = 'warehouse_id_example' # str | 
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    stock_adjustment = simplebilly_api.StockAdjustment() # StockAdjustment | 

    try:
        api_response = api_instance.update_warehouse_stock(warehouse_id, product_id, stock_adjustment)
        print("The response of WarehouseStockApi->update_warehouse_stock:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WarehouseStockApi->update_warehouse_stock: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouse_id** | **str**|  | 
 **product_id** | **UUID**|  | 
 **stock_adjustment** | [**StockAdjustment**](StockAdjustment.md)|  | 

### Return type

[**WarehouseStock**](WarehouseStock.md)

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

