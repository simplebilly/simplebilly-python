# simplebilly_api.ReorderProposalApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apply_reorder_proposal**](ReorderProposalApi.md#apply_reorder_proposal) | **POST** /api/v1/reorder-proposals/apply | Convert a reorder proposal into a draft purchase order.
[**get_reorder_proposal**](ReorderProposalApi.md#get_reorder_proposal) | **GET** /api/v1/reorder-proposals | 


# **apply_reorder_proposal**
> object apply_reorder_proposal(configured_only=configured_only, warehouse_id=warehouse_id)

Convert a reorder proposal into a draft purchase order.

Returns the created purchase order id. Suggested line items are generated
with the current reorder quantity per product.

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
    api_instance = simplebilly_api.ReorderProposalApi(api_client)
    configured_only = True # bool | Only include products with a reorder point configured (`min_stock`). (optional)
    warehouse_id = 'warehouse_id_example' # str | Limit to a single warehouse id. (optional)

    try:
        # Convert a reorder proposal into a draft purchase order.
        api_response = api_instance.apply_reorder_proposal(configured_only=configured_only, warehouse_id=warehouse_id)
        print("The response of ReorderProposalApi->apply_reorder_proposal:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReorderProposalApi->apply_reorder_proposal: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **configured_only** | **bool**| Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [optional] 
 **warehouse_id** | **str**| Limit to a single warehouse id. | [optional] 

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

# **get_reorder_proposal**
> ReorderProposalResponse get_reorder_proposal(configured_only=configured_only, warehouse_id=warehouse_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.reorder_proposal_response import ReorderProposalResponse
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
    api_instance = simplebilly_api.ReorderProposalApi(api_client)
    configured_only = True # bool | Only include products with a reorder point configured (`min_stock`). (optional)
    warehouse_id = 'warehouse_id_example' # str | Limit to a single warehouse id. (optional)

    try:
        api_response = api_instance.get_reorder_proposal(configured_only=configured_only, warehouse_id=warehouse_id)
        print("The response of ReorderProposalApi->get_reorder_proposal:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReorderProposalApi->get_reorder_proposal: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **configured_only** | **bool**| Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [optional] 
 **warehouse_id** | **str**| Limit to a single warehouse id. | [optional] 

### Return type

[**ReorderProposalResponse**](ReorderProposalResponse.md)

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

