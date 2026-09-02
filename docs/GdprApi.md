# simplebilly_api.GdprApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**accept_dpa**](GdprApi.md#accept_dpa) | **PUT** /api/v1/gdpr/dpa | Record DPA acceptance: sets dpa_accepted_at/by/version on the tenant settings row (created with company-type defaults if missing).
[**account_erasure**](GdprApi.md#account_erasure) | **POST** /api/v1/gdpr/account-erasure | Erase ALL personal data of the tenant (TOS §11: deletion 90 days after termination).
[**erasure_contact**](GdprApi.md#erasure_contact) | **POST** /api/v1/gdpr/erasure/{contact_id} | Anonymize + soft-delete a contact: personal attributes are cleared, the record itself is kept for GoBD retention (Art. 17(3)(e) DSGVO). The audit trigger on &#x60;contacts&#x60; already records who/when.
[**export_contact_data**](GdprApi.md#export_contact_data) | **GET** /api/v1/gdpr/export/{contact_id} | Art. 15 data-subject access export for a contact.
[**export_gdpr**](GdprApi.md#export_gdpr) | **GET** /api/v1/gdpr/export | Export the current user&#39;s personal data (GDPR Art. 15/20).
[**get_dpa**](GdprApi.md#get_dpa) | **GET** /api/v1/gdpr/dpa | Current DPA acceptance status (from tenant_settings).


# **accept_dpa**
> DpaStatus accept_dpa(dpa_accept_request)

Record DPA acceptance: sets dpa_accepted_at/by/version on the tenant settings row (created with company-type defaults if missing).

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.dpa_accept_request import DpaAcceptRequest
from simplebilly_api.models.dpa_status import DpaStatus
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
    api_instance = simplebilly_api.GdprApi(api_client)
    dpa_accept_request = simplebilly_api.DpaAcceptRequest() # DpaAcceptRequest | 

    try:
        # Record DPA acceptance: sets dpa_accepted_at/by/version on the tenant settings row (created with company-type defaults if missing).
        api_response = api_instance.accept_dpa(dpa_accept_request)
        print("The response of GdprApi->accept_dpa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GdprApi->accept_dpa: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dpa_accept_request** | [**DpaAcceptRequest**](DpaAcceptRequest.md)|  | 

### Return type

[**DpaStatus**](DpaStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | DPA acceptance recorded |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **account_erasure**
> object account_erasure()

Erase ALL personal data of the tenant (TOS §11: deletion 90 days after termination).

Anonymizes every contact, anonymizes personal fields on bookkeeping
records (orders/invoices/payments keep amounts and dates for GoBD),
removes the tenant linkage of the (global, saasy-framework) users and
marks the erasure on `tenant_settings.gdpr_erased_at`. No row is
physically deleted. The audit triggers on the touched tables record
who/when.

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
    api_instance = simplebilly_api.GdprApi(api_client)

    try:
        # Erase ALL personal data of the tenant (TOS §11: deletion 90 days after termination).
        api_response = api_instance.account_erasure()
        print("The response of GdprApi->account_erasure:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GdprApi->account_erasure: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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
**200** | Tenant personal data anonymized |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **erasure_contact**
> object erasure_contact(contact_id)

Anonymize + soft-delete a contact: personal attributes are cleared, the record itself is kept for GoBD retention (Art. 17(3)(e) DSGVO). The audit trigger on `contacts` already records who/when.

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
    api_instance = simplebilly_api.GdprApi(api_client)
    contact_id = 'contact_id_example' # str | 

    try:
        # Anonymize + soft-delete a contact: personal attributes are cleared, the record itself is kept for GoBD retention (Art. 17(3)(e) DSGVO). The audit trigger on `contacts` already records who/when.
        api_response = api_instance.erasure_contact(contact_id)
        print("The response of GdprApi->erasure_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GdprApi->erasure_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contact_id** | **str**|  | 

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
**200** | Contact anonymized |  -  |
**404** | Contact not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_contact_data**
> object export_contact_data(contact_id)

Art. 15 data-subject access export for a contact.

Returns the contact itself plus the tenant-scoped rows linked to it.

## Relations
The `customers`/`orders`/`invoices`/`payments` tables have no FK to
`contacts`; they are linked through the `customer_id` column, which per
the app's conventions holds one of:
- the admin customer's `customer_id` (a UUID, often the same value as
  the contact's `contact_id`/`customer_number`),
- the buyer's email for shop orders, or
- the marketplace's external customer id for plugin orders.

The export therefore matches the contact's identifiers (`contact_id`,
`customer_number`, `external_id`, `email`) plus any resolved customer ids
against `customer_id`. `delivery_notes` and `customer_communications`
reference contacts directly via `contact_id`. Soft-deleted rows are
included (their data is still processed and retained for GoBD).
Relations that genuinely do not exist for a contact stay empty but the
key is always present.

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
    api_instance = simplebilly_api.GdprApi(api_client)
    contact_id = 'contact_id_example' # str | 

    try:
        # Art. 15 data-subject access export for a contact.
        api_response = api_instance.export_contact_data(contact_id)
        print("The response of GdprApi->export_contact_data:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GdprApi->export_contact_data: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contact_id** | **str**|  | 

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
**200** | Art. 15 data-subject export |  -  |
**404** | Contact not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_gdpr**
> ApiResponseGdprExport export_gdpr()

Export the current user's personal data (GDPR Art. 15/20).

No admin permission required: a user always exports their own data.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.api_response_gdpr_export import ApiResponseGdprExport
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
    api_instance = simplebilly_api.GdprApi(api_client)

    try:
        # Export the current user's personal data (GDPR Art. 15/20).
        api_response = api_instance.export_gdpr()
        print("The response of GdprApi->export_gdpr:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GdprApi->export_gdpr: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiResponseGdprExport**](ApiResponseGdprExport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Personal data export |  -  |
**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_dpa**
> DpaStatus get_dpa()

Current DPA acceptance status (from tenant_settings).

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.dpa_status import DpaStatus
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
    api_instance = simplebilly_api.GdprApi(api_client)

    try:
        # Current DPA acceptance status (from tenant_settings).
        api_response = api_instance.get_dpa()
        print("The response of GdprApi->get_dpa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GdprApi->get_dpa: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**DpaStatus**](DpaStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | DPA acceptance status |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

