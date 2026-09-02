# simplebilly_api.DeliveryAppointmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_delivery_appointment**](DeliveryAppointmentApi.md#create_delivery_appointment) | **POST** /api/v1/delivery-appointments | 
[**delete_delivery_appointment**](DeliveryAppointmentApi.md#delete_delivery_appointment) | **DELETE** /api/v1/delivery-appointments/{appointment_id} | 
[**get_delivery_appointment**](DeliveryAppointmentApi.md#get_delivery_appointment) | **GET** /api/v1/delivery-appointments/{appointment_id} | 
[**get_public_delivery_appointment_status**](DeliveryAppointmentApi.md#get_public_delivery_appointment_status) | **GET** /api/v1/public/delivery-appointments/status | Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.
[**list_delivery_appointments**](DeliveryAppointmentApi.md#list_delivery_appointments) | **GET** /api/v1/delivery-appointments | 
[**request_public_delivery_appointment**](DeliveryAppointmentApi.md#request_public_delivery_appointment) | **POST** /api/v1/public/delivery-appointments/request | Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request.
[**update_delivery_appointment**](DeliveryAppointmentApi.md#update_delivery_appointment) | **PUT** /api/v1/delivery-appointments/{appointment_id} | 
[**update_delivery_appointment_status**](DeliveryAppointmentApi.md#update_delivery_appointment_status) | **PUT** /api/v1/delivery-appointments/{appointment_id}/status | 


# **create_delivery_appointment**
> DeliveryAppointment create_delivery_appointment(delivery_appointment_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.delivery_appointment import DeliveryAppointment
from simplebilly_api.models.delivery_appointment_create import DeliveryAppointmentCreate
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
    api_instance = simplebilly_api.DeliveryAppointmentApi(api_client)
    delivery_appointment_create = simplebilly_api.DeliveryAppointmentCreate() # DeliveryAppointmentCreate | 

    try:
        api_response = api_instance.create_delivery_appointment(delivery_appointment_create)
        print("The response of DeliveryAppointmentApi->create_delivery_appointment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryAppointmentApi->create_delivery_appointment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **delivery_appointment_create** | [**DeliveryAppointmentCreate**](DeliveryAppointmentCreate.md)|  | 

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

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

# **delete_delivery_appointment**
> delete_delivery_appointment(appointment_id)

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
    api_instance = simplebilly_api.DeliveryAppointmentApi(api_client)
    appointment_id = 'appointment_id_example' # str | 

    try:
        api_instance.delete_delivery_appointment(appointment_id)
    except Exception as e:
        print("Exception when calling DeliveryAppointmentApi->delete_delivery_appointment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointment_id** | **str**|  | 

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

# **get_delivery_appointment**
> DeliveryAppointment get_delivery_appointment(appointment_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.delivery_appointment import DeliveryAppointment
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
    api_instance = simplebilly_api.DeliveryAppointmentApi(api_client)
    appointment_id = 'appointment_id_example' # str | 

    try:
        api_response = api_instance.get_delivery_appointment(appointment_id)
        print("The response of DeliveryAppointmentApi->get_delivery_appointment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryAppointmentApi->get_delivery_appointment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointment_id** | **str**|  | 

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

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

# **get_public_delivery_appointment_status**
> PublicDeliveryAppointmentStatusResponse get_public_delivery_appointment_status(appointment_id, email, token)

Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.public_delivery_appointment_status_response import PublicDeliveryAppointmentStatusResponse
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
    api_instance = simplebilly_api.DeliveryAppointmentApi(api_client)
    appointment_id = 'appointment_id_example' # str | 
    email = 'email_example' # str | 
    token = 'token_example' # str | 

    try:
        # Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.
        api_response = api_instance.get_public_delivery_appointment_status(appointment_id, email, token)
        print("The response of DeliveryAppointmentApi->get_public_delivery_appointment_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryAppointmentApi->get_public_delivery_appointment_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointment_id** | **str**|  | 
 **email** | **str**|  | 
 **token** | **str**|  | 

### Return type

[**PublicDeliveryAppointmentStatusResponse**](PublicDeliveryAppointmentStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Appointment status |  -  |
**404** | Appointment not found or credentials mismatch |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_delivery_appointments**
> List[DeliveryAppointment] list_delivery_appointments(page=page, page_size=page_size, status=status, warehouse_id=warehouse_id, var_from=var_from, to=to)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.delivery_appointment import DeliveryAppointment
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
    api_instance = simplebilly_api.DeliveryAppointmentApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    status = 'status_example' # str |  (optional)
    warehouse_id = 'warehouse_id_example' # str |  (optional)
    var_from = '2013-10-20' # date |  (optional)
    to = '2013-10-20' # date |  (optional)

    try:
        api_response = api_instance.list_delivery_appointments(page=page, page_size=page_size, status=status, warehouse_id=warehouse_id, var_from=var_from, to=to)
        print("The response of DeliveryAppointmentApi->list_delivery_appointments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryAppointmentApi->list_delivery_appointments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **status** | **str**|  | [optional] 
 **warehouse_id** | **str**|  | [optional] 
 **var_from** | **date**|  | [optional] 
 **to** | **date**|  | [optional] 

### Return type

[**List[DeliveryAppointment]**](DeliveryAppointment.md)

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

# **request_public_delivery_appointment**
> PublicDeliveryAppointmentResponse request_public_delivery_appointment(public_delivery_appointment_request)

Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by `code` — never from the request.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.public_delivery_appointment_request import PublicDeliveryAppointmentRequest
from simplebilly_api.models.public_delivery_appointment_response import PublicDeliveryAppointmentResponse
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
    api_instance = simplebilly_api.DeliveryAppointmentApi(api_client)
    public_delivery_appointment_request = simplebilly_api.PublicDeliveryAppointmentRequest() # PublicDeliveryAppointmentRequest | 

    try:
        # Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by `code` — never from the request.
        api_response = api_instance.request_public_delivery_appointment(public_delivery_appointment_request)
        print("The response of DeliveryAppointmentApi->request_public_delivery_appointment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryAppointmentApi->request_public_delivery_appointment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **public_delivery_appointment_request** | [**PublicDeliveryAppointmentRequest**](PublicDeliveryAppointmentRequest.md)|  | 

### Return type

[**PublicDeliveryAppointmentResponse**](PublicDeliveryAppointmentResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Appointment requested |  -  |
**404** | Warehouse not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_delivery_appointment**
> DeliveryAppointment update_delivery_appointment(appointment_id, body)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.delivery_appointment import DeliveryAppointment
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
    api_instance = simplebilly_api.DeliveryAppointmentApi(api_client)
    appointment_id = 'appointment_id_example' # str | 
    body = None # object | 

    try:
        api_response = api_instance.update_delivery_appointment(appointment_id, body)
        print("The response of DeliveryAppointmentApi->update_delivery_appointment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryAppointmentApi->update_delivery_appointment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointment_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad request |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_delivery_appointment_status**
> DeliveryAppointment update_delivery_appointment_status(appointment_id, appointment_status_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.appointment_status_update import AppointmentStatusUpdate
from simplebilly_api.models.delivery_appointment import DeliveryAppointment
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
    api_instance = simplebilly_api.DeliveryAppointmentApi(api_client)
    appointment_id = 'appointment_id_example' # str | 
    appointment_status_update = simplebilly_api.AppointmentStatusUpdate() # AppointmentStatusUpdate | 

    try:
        api_response = api_instance.update_delivery_appointment_status(appointment_id, appointment_status_update)
        print("The response of DeliveryAppointmentApi->update_delivery_appointment_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DeliveryAppointmentApi->update_delivery_appointment_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointment_id** | **str**|  | 
 **appointment_status_update** | [**AppointmentStatusUpdate**](AppointmentStatusUpdate.md)|  | 

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad request / invalid transition |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

