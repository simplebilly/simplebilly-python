# simplebilly_api.AttachmentVersionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_attachment_version**](AttachmentVersionApi.md#create_attachment_version) | **POST** /api/v1/attachments/{attachment_id}/versions | 
[**list_attachment_versions**](AttachmentVersionApi.md#list_attachment_versions) | **GET** /api/v1/attachments/{attachment_id}/versions | 
[**restore_attachment_version**](AttachmentVersionApi.md#restore_attachment_version) | **POST** /api/v1/attachments/{attachment_id}/versions/{version_id}/restore | 


# **create_attachment_version**
> AttachmentVersion create_attachment_version(attachment_id, new_version_request)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.attachment_version import AttachmentVersion
from simplebilly_api.models.new_version_request import NewVersionRequest
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
    api_instance = simplebilly_api.AttachmentVersionApi(api_client)
    attachment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    new_version_request = simplebilly_api.NewVersionRequest() # NewVersionRequest | 

    try:
        api_response = api_instance.create_attachment_version(attachment_id, new_version_request)
        print("The response of AttachmentVersionApi->create_attachment_version:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentVersionApi->create_attachment_version: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attachment_id** | **UUID**|  | 
 **new_version_request** | [**NewVersionRequest**](NewVersionRequest.md)|  | 

### Return type

[**AttachmentVersion**](AttachmentVersion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | New current version recorded |  -  |
**400** | Bad request |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_attachment_versions**
> List[AttachmentVersion] list_attachment_versions(attachment_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.attachment_version import AttachmentVersion
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
    api_instance = simplebilly_api.AttachmentVersionApi(api_client)
    attachment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_response = api_instance.list_attachment_versions(attachment_id)
        print("The response of AttachmentVersionApi->list_attachment_versions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentVersionApi->list_attachment_versions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attachment_id** | **UUID**|  | 

### Return type

[**List[AttachmentVersion]**](AttachmentVersion.md)

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

# **restore_attachment_version**
> Attachment restore_attachment_version(attachment_id, version_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.attachment import Attachment
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
    api_instance = simplebilly_api.AttachmentVersionApi(api_client)
    attachment_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    version_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        api_response = api_instance.restore_attachment_version(attachment_id, version_id)
        print("The response of AttachmentVersionApi->restore_attachment_version:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AttachmentVersionApi->restore_attachment_version: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attachment_id** | **UUID**|  | 
 **version_id** | **UUID**|  | 

### Return type

[**Attachment**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Attachment restored |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

