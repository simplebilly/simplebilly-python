# simplebilly_api.InstituteProfileApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_institute_profile**](InstituteProfileApi.md#get_institute_profile) | **GET** /api/v1/institute-profile | Current institute profile (created with defaults when missing).
[**update_institute_profile**](InstituteProfileApi.md#update_institute_profile) | **PUT** /api/v1/institute-profile | Update the institute profile (institute_type and/or kapitalmarktorientiert).


# **get_institute_profile**
> InstituteProfile get_institute_profile()

Current institute profile (created with defaults when missing).

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.institute_profile import InstituteProfile
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
    api_instance = simplebilly_api.InstituteProfileApi(api_client)

    try:
        # Current institute profile (created with defaults when missing).
        api_response = api_instance.get_institute_profile()
        print("The response of InstituteProfileApi->get_institute_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstituteProfileApi->get_institute_profile: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**InstituteProfile**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Institute profile |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_institute_profile**
> InstituteProfile update_institute_profile(institute_profile_update)

Update the institute profile (institute_type and/or kapitalmarktorientiert).

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.institute_profile import InstituteProfile
from simplebilly_api.models.institute_profile_update import InstituteProfileUpdate
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
    api_instance = simplebilly_api.InstituteProfileApi(api_client)
    institute_profile_update = simplebilly_api.InstituteProfileUpdate() # InstituteProfileUpdate | 

    try:
        # Update the institute profile (institute_type and/or kapitalmarktorientiert).
        api_response = api_instance.update_institute_profile(institute_profile_update)
        print("The response of InstituteProfileApi->update_institute_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InstituteProfileApi->update_institute_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **institute_profile_update** | [**InstituteProfileUpdate**](InstituteProfileUpdate.md)|  | 

### Return type

[**InstituteProfile**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated institute profile |  -  |
**400** | Invalid institute_type |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

