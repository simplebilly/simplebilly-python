# simplebilly_api.WorkflowsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_workflows_api**](WorkflowsApi.md#list_workflows_api) | **GET** /api/v1/workflows | 
[**set_workflow_enabled_api**](WorkflowsApi.md#set_workflow_enabled_api) | **PUT** /api/v1/workflows/{workflow_id}/enabled | 


# **list_workflows_api**
> List[Workflow] list_workflows_api()

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.workflow import Workflow
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
    api_instance = simplebilly_api.WorkflowsApi(api_client)

    try:
        api_response = api_instance.list_workflows_api()
        print("The response of WorkflowsApi->list_workflows_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkflowsApi->list_workflows_api: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[Workflow]**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Workflows (seeded with defaults on first access) |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **set_workflow_enabled_api**
> Workflow set_workflow_enabled_api(workflow_id, workflow_enabled_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.workflow import Workflow
from simplebilly_api.models.workflow_enabled_update import WorkflowEnabledUpdate
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
    api_instance = simplebilly_api.WorkflowsApi(api_client)
    workflow_id = 'workflow_id_example' # str | 
    workflow_enabled_update = simplebilly_api.WorkflowEnabledUpdate() # WorkflowEnabledUpdate | 

    try:
        api_response = api_instance.set_workflow_enabled_api(workflow_id, workflow_enabled_update)
        print("The response of WorkflowsApi->set_workflow_enabled_api:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkflowsApi->set_workflow_enabled_api: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workflow_id** | **str**|  | 
 **workflow_enabled_update** | [**WorkflowEnabledUpdate**](WorkflowEnabledUpdate.md)|  | 

### Return type

[**Workflow**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Workflow enabled state updated |  -  |
**404** | Workflow not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

