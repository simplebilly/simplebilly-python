# simplebilly_api.LeadApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_leads_api**](LeadApi.md#list_leads_api) | **GET** /api/v1/support/leads | 
[**update_lead_api**](LeadApi.md#update_lead_api) | **PUT** /api/v1/support/leads/{lead_id} | 


# **list_leads_api**
> List[Lead] list_leads_api(status=status, source=source, search=search, page=page, page_size=page_size)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.lead import Lead
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
    api_instance = simplebilly_api.LeadApi(api_client)
    status = 'status_example' # str |  (optional)
    source = 'source_example' # str |  (optional)
    search = 'search_example' # str |  (optional)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)

    try:
        api_response = api_instance.list_leads_api(status=status, source=source, search=search, page=page, page_size=page_size)
        print("The response of LeadApi->list_leads_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LeadApi->list_leads_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **str**|  | [optional] 
 **source** | **str**|  | [optional] 
 **search** | **str**|  | [optional] 
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 

### Return type

[**List[Lead]**](Lead.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Leads list |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_lead_api**
> Lead update_lead_api(lead_id, lead_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.lead import Lead
from simplebilly_api.models.lead_update import LeadUpdate
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
    api_instance = simplebilly_api.LeadApi(api_client)
    lead_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    lead_update = simplebilly_api.LeadUpdate() # LeadUpdate | 

    try:
        api_response = api_instance.update_lead_api(lead_id, lead_update)
        print("The response of LeadApi->update_lead_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LeadApi->update_lead_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lead_id** | **UUID**|  | 
 **lead_update** | [**LeadUpdate**](LeadUpdate.md)|  | 

### Return type

[**Lead**](Lead.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Lead updated |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

