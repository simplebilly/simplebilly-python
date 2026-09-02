# simplebilly_api.TimeEntriesApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**clock_in_time_entry**](TimeEntriesApi.md#clock_in_time_entry) | **POST** /api/v1/time-entries | Clock in for the authenticated user (resolved via their employee profile).
[**clock_out_time_entry**](TimeEntriesApi.md#clock_out_time_entry) | **PATCH** /api/v1/time-entries/{id} | Clock out an entry: the entry&#39;s owner, or anyone with &#x60;time_entries:write&#x60;.
[**get_labor_costs**](TimeEntriesApi.md#get_labor_costs) | **GET** /api/v1/labor-costs | Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee&#39;s hourly cost rate.
[**list_time_entries**](TimeEntriesApi.md#list_time_entries) | **GET** /api/v1/time-entries | List time entries with optional date-range / active / employee filters.


# **clock_in_time_entry**
> TimeEntryDto clock_in_time_entry(time_entry_clock_in)

Clock in for the authenticated user (resolved via their employee profile).

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.time_entry_clock_in import TimeEntryClockIn
from simplebilly_api.models.time_entry_dto import TimeEntryDto
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
    api_instance = simplebilly_api.TimeEntriesApi(api_client)
    time_entry_clock_in = simplebilly_api.TimeEntryClockIn() # TimeEntryClockIn | 

    try:
        # Clock in for the authenticated user (resolved via their employee profile).
        api_response = api_instance.clock_in_time_entry(time_entry_clock_in)
        print("The response of TimeEntriesApi->clock_in_time_entry:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TimeEntriesApi->clock_in_time_entry: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **time_entry_clock_in** | [**TimeEntryClockIn**](TimeEntryClockIn.md)|  | 

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | No employee profile for this user |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **clock_out_time_entry**
> TimeEntryDto clock_out_time_entry(id, time_entry_clock_out)

Clock out an entry: the entry's owner, or anyone with `time_entries:write`.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.time_entry_clock_out import TimeEntryClockOut
from simplebilly_api.models.time_entry_dto import TimeEntryDto
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
    api_instance = simplebilly_api.TimeEntriesApi(api_client)
    id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 
    time_entry_clock_out = simplebilly_api.TimeEntryClockOut() # TimeEntryClockOut | 

    try:
        # Clock out an entry: the entry's owner, or anyone with `time_entries:write`.
        api_response = api_instance.clock_out_time_entry(id, time_entry_clock_out)
        print("The response of TimeEntriesApi->clock_out_time_entry:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TimeEntriesApi->clock_out_time_entry: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | 
 **time_entry_clock_out** | [**TimeEntryClockOut**](TimeEntryClockOut.md)|  | 

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

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
**403** | Forbidden |  -  |
**404** | Not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_labor_costs**
> List[LaborCostRow] get_labor_costs(var_from, to, group_by)

Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee's hourly cost rate.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.labor_cost_row import LaborCostRow
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
    api_instance = simplebilly_api.TimeEntriesApi(api_client)
    var_from = '2013-10-20' # date | 
    to = '2013-10-20' # date | 
    group_by = 'group_by_example' # str | One of \"employee\", \"order\" or \"day\".

    try:
        # Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee's hourly cost rate.
        api_response = api_instance.get_labor_costs(var_from, to, group_by)
        print("The response of TimeEntriesApi->get_labor_costs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TimeEntriesApi->get_labor_costs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **var_from** | **date**|  | 
 **to** | **date**|  | 
 **group_by** | **str**| One of \&quot;employee\&quot;, \&quot;order\&quot; or \&quot;day\&quot;. | 

### Return type

[**List[LaborCostRow]**](LaborCostRow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad request |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_time_entries**
> List[TimeEntryDto] list_time_entries(var_from=var_from, to=to, active=active, employee_id=employee_id)

List time entries with optional date-range / active / employee filters.

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.time_entry_dto import TimeEntryDto
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
    api_instance = simplebilly_api.TimeEntriesApi(api_client)
    var_from = '2013-10-20' # date |  (optional)
    to = '2013-10-20' # date |  (optional)
    active = True # bool | Only currently running shifts (clock_in set, clock_out null). (optional)
    employee_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID |  (optional)

    try:
        # List time entries with optional date-range / active / employee filters.
        api_response = api_instance.list_time_entries(var_from=var_from, to=to, active=active, employee_id=employee_id)
        print("The response of TimeEntriesApi->list_time_entries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TimeEntriesApi->list_time_entries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **var_from** | **date**|  | [optional] 
 **to** | **date**|  | [optional] 
 **active** | **bool**| Only currently running shifts (clock_in set, clock_out null). | [optional] 
 **employee_id** | **UUID**|  | [optional] 

### Return type

[**List[TimeEntryDto]**](TimeEntryDto.md)

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

