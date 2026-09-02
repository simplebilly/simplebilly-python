# simplebilly_api.ReplenishmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apply_replenishments**](ReplenishmentApi.md#apply_replenishments) | **POST** /api/v1/replenishments/apply | Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.
[**get_replenishments**](ReplenishmentApi.md#get_replenishments) | **GET** /api/v1/replenishments | 


# **apply_replenishments**
> object apply_replenishments(target_warehouse_id=target_warehouse_id, source_warehouse_id=source_warehouse_id)

Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.

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
    api_instance = simplebilly_api.ReplenishmentApi(api_client)
    target_warehouse_id = 'target_warehouse_id_example' # str | Warehouse to be replenished. Defaults to the tenant's default warehouse. (optional)
    source_warehouse_id = 'source_warehouse_id_example' # str | Restrict source warehouses to this id. (optional)

    try:
        # Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.
        api_response = api_instance.apply_replenishments(target_warehouse_id=target_warehouse_id, source_warehouse_id=source_warehouse_id)
        print("The response of ReplenishmentApi->apply_replenishments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReplenishmentApi->apply_replenishments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **target_warehouse_id** | **str**| Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [optional] 
 **source_warehouse_id** | **str**| Restrict source warehouses to this id. | [optional] 

### Return type

**object**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | Bad request |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_replenishments**
> ReplenishmentResponse get_replenishments(target_warehouse_id=target_warehouse_id, source_warehouse_id=source_warehouse_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.replenishment_response import ReplenishmentResponse
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
    api_instance = simplebilly_api.ReplenishmentApi(api_client)
    target_warehouse_id = 'target_warehouse_id_example' # str | Warehouse to be replenished. Defaults to the tenant's default warehouse. (optional)
    source_warehouse_id = 'source_warehouse_id_example' # str | Restrict source warehouses to this id. (optional)

    try:
        api_response = api_instance.get_replenishments(target_warehouse_id=target_warehouse_id, source_warehouse_id=source_warehouse_id)
        print("The response of ReplenishmentApi->get_replenishments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReplenishmentApi->get_replenishments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **target_warehouse_id** | **str**| Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [optional] 
 **source_warehouse_id** | **str**| Restrict source warehouses to this id. | [optional] 

### Return type

[**ReplenishmentResponse**](ReplenishmentResponse.md)

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

