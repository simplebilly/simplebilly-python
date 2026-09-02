# simplebilly_api.StockMovementApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_stock_movement**](StockMovementApi.md#get_stock_movement) | **GET** /api/v1/stock-movements/{movement_id} | 
[**list_stock_movements**](StockMovementApi.md#list_stock_movements) | **GET** /api/v1/stock-movements/ | 


# **get_stock_movement**
> StockMovement get_stock_movement(movement_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.stock_movement import StockMovement
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
    api_instance = simplebilly_api.StockMovementApi(api_client)
    movement_id = 'movement_id_example' # str | 

    try:
        api_response = api_instance.get_stock_movement(movement_id)
        print("The response of StockMovementApi->get_stock_movement:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StockMovementApi->get_stock_movement: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **movement_id** | **str**|  | 

### Return type

[**StockMovement**](StockMovement.md)

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

# **list_stock_movements**
> List[StockMovement] list_stock_movements(page=page, page_size=page_size, product_id=product_id, warehouse_id=warehouse_id, movement_type=movement_type, var_from=var_from, to=to)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.stock_movement import StockMovement
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
    api_instance = simplebilly_api.StockMovementApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    product_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)
    warehouse_id = 'warehouse_id_example' # str |  (optional)
    movement_type = 'movement_type_example' # str |  (optional)
    var_from = '2013-10-20' # date | Only movements on or after this date (inclusive). (optional)
    to = '2013-10-20' # date | Only movements on or before this date (inclusive). (optional)

    try:
        api_response = api_instance.list_stock_movements(page=page, page_size=page_size, product_id=product_id, warehouse_id=warehouse_id, movement_type=movement_type, var_from=var_from, to=to)
        print("The response of StockMovementApi->list_stock_movements:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StockMovementApi->list_stock_movements: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **product_id** | **UUID**|  | [optional] 
 **warehouse_id** | **str**|  | [optional] 
 **movement_type** | **str**|  | [optional] 
 **var_from** | **date**| Only movements on or after this date (inclusive). | [optional] 
 **to** | **date**| Only movements on or before this date (inclusive). | [optional] 

### Return type

[**List[StockMovement]**](StockMovement.md)

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

