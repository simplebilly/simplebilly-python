# simplebilly_api.LegalDocumentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_legal_documents**](LegalDocumentApi.md#get_legal_documents) | **GET** /api/v1/legal/documents | List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.
[**reset_legal_documents**](LegalDocumentApi.md#reset_legal_documents) | **POST** /api/v1/legal/documents/reset | Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.
[**upsert_legal_documents**](LegalDocumentApi.md#upsert_legal_documents) | **PUT** /api/v1/legal/documents | Upsert legal documents per (doc_type, lang). Returns the full tenant list.


# **get_legal_documents**
> List[LegalDocument] get_legal_documents()

List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.legal_document import LegalDocument
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
    api_instance = simplebilly_api.LegalDocumentApi(api_client)

    try:
        # List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.
        api_response = api_instance.get_legal_documents()
        print("The response of LegalDocumentApi->get_legal_documents:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LegalDocumentApi->get_legal_documents: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[LegalDocument]**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | All legal documents of the tenant |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reset_legal_documents**
> List[LegalDocument] reset_legal_documents(legal_document_reset)

Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.legal_document import LegalDocument
from simplebilly_api.models.legal_document_reset import LegalDocumentReset
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
    api_instance = simplebilly_api.LegalDocumentApi(api_client)
    legal_document_reset = simplebilly_api.LegalDocumentReset() # LegalDocumentReset | 

    try:
        # Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.
        api_response = api_instance.reset_legal_documents(legal_document_reset)
        print("The response of LegalDocumentApi->reset_legal_documents:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LegalDocumentApi->reset_legal_documents: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **legal_document_reset** | [**LegalDocumentReset**](LegalDocumentReset.md)|  | 

### Return type

[**List[LegalDocument]**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Reset legal documents |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upsert_legal_documents**
> List[LegalDocument] upsert_legal_documents(legal_document_upsert)

Upsert legal documents per (doc_type, lang). Returns the full tenant list.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.legal_document import LegalDocument
from simplebilly_api.models.legal_document_upsert import LegalDocumentUpsert
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
    api_instance = simplebilly_api.LegalDocumentApi(api_client)
    legal_document_upsert = [simplebilly_api.LegalDocumentUpsert()] # List[LegalDocumentUpsert] | 

    try:
        # Upsert legal documents per (doc_type, lang). Returns the full tenant list.
        api_response = api_instance.upsert_legal_documents(legal_document_upsert)
        print("The response of LegalDocumentApi->upsert_legal_documents:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LegalDocumentApi->upsert_legal_documents: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **legal_document_upsert** | [**List[LegalDocumentUpsert]**](LegalDocumentUpsert.md)|  | 

### Return type

[**List[LegalDocument]**](LegalDocument.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Saved legal documents |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

