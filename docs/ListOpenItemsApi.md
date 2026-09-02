# simplebilly_api.ListOpenItemsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_open_items_api**](ListOpenItemsApi.md#list_open_items_api) | **GET** /api/v1/bookkeeping/open-items | 


# **list_open_items_api**
> List[OpenItem] list_open_items_api(reminder_level1_days=reminder_level1_days, reminder_level2_days=reminder_level2_days, reminder_level3_days=reminder_level3_days, customer_id=customer_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.open_item import OpenItem
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
    api_instance = simplebilly_api.ListOpenItemsApi(api_client)
    reminder_level1_days = 56 # int |  (optional)
    reminder_level2_days = 56 # int |  (optional)
    reminder_level3_days = 56 # int |  (optional)
    customer_id = 'customer_id_example' # str |  (optional)

    try:
        api_response = api_instance.list_open_items_api(reminder_level1_days=reminder_level1_days, reminder_level2_days=reminder_level2_days, reminder_level3_days=reminder_level3_days, customer_id=customer_id)
        print("The response of ListOpenItemsApi->list_open_items_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ListOpenItemsApi->list_open_items_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **reminder_level1_days** | **int**|  | [optional] 
 **reminder_level2_days** | **int**|  | [optional] 
 **reminder_level3_days** | **int**|  | [optional] 
 **customer_id** | **str**|  | [optional] 

### Return type

[**List[OpenItem]**](OpenItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of open invoices |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

