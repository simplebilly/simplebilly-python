# simplebilly_api.ShippingRuleApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_rule**](ShippingRuleApi.md#create_shipping_rule) | **POST** /api/v1/shipping-rules | 
[**delete_shipping_rule**](ShippingRuleApi.md#delete_shipping_rule) | **DELETE** /api/v1/shipping-rules/{rule_id} | 
[**get_shipping_rule**](ShippingRuleApi.md#get_shipping_rule) | **GET** /api/v1/shipping-rules/{rule_id} | 
[**list_shipping_rules**](ShippingRuleApi.md#list_shipping_rules) | **GET** /api/v1/shipping-rules/ | 
[**update_shipping_rule**](ShippingRuleApi.md#update_shipping_rule) | **PUT** /api/v1/shipping-rules/{rule_id} | 


# **create_shipping_rule**
> ShippingRule create_shipping_rule(shipping_rule_create)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.shipping_rule import ShippingRule
from simplebilly_api.models.shipping_rule_create import ShippingRuleCreate
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
    api_instance = simplebilly_api.ShippingRuleApi(api_client)
    shipping_rule_create = simplebilly_api.ShippingRuleCreate() # ShippingRuleCreate | 

    try:
        api_response = api_instance.create_shipping_rule(shipping_rule_create)
        print("The response of ShippingRuleApi->create_shipping_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShippingRuleApi->create_shipping_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipping_rule_create** | [**ShippingRuleCreate**](ShippingRuleCreate.md)|  | 

### Return type

[**ShippingRule**](ShippingRule.md)

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

# **delete_shipping_rule**
> delete_shipping_rule(rule_id)

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
    api_instance = simplebilly_api.ShippingRuleApi(api_client)
    rule_id = 'rule_id_example' # str | 

    try:
        api_instance.delete_shipping_rule(rule_id)
    except Exception as e:
        print("Exception when calling ShippingRuleApi->delete_shipping_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **str**|  | 

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

# **get_shipping_rule**
> ShippingRule get_shipping_rule(rule_id)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.shipping_rule import ShippingRule
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
    api_instance = simplebilly_api.ShippingRuleApi(api_client)
    rule_id = 'rule_id_example' # str | 

    try:
        api_response = api_instance.get_shipping_rule(rule_id)
        print("The response of ShippingRuleApi->get_shipping_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShippingRuleApi->get_shipping_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **str**|  | 

### Return type

[**ShippingRule**](ShippingRule.md)

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

# **list_shipping_rules**
> List[ShippingRule] list_shipping_rules(page=page, page_size=page_size, country=country)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.shipping_rule import ShippingRule
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
    api_instance = simplebilly_api.ShippingRuleApi(api_client)
    page = 56 # int |  (optional)
    page_size = 56 # int |  (optional)
    country = 'country_example' # str |  (optional)

    try:
        api_response = api_instance.list_shipping_rules(page=page, page_size=page_size, country=country)
        print("The response of ShippingRuleApi->list_shipping_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShippingRuleApi->list_shipping_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] 
 **page_size** | **int**|  | [optional] 
 **country** | **str**|  | [optional] 

### Return type

[**List[ShippingRule]**](ShippingRule.md)

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

# **update_shipping_rule**
> ShippingRule update_shipping_rule(rule_id, shipping_rule_update)

### Example

* Bearer (JWT) Authentication (bearer_token):

```python
import simplebilly_api
from simplebilly_api.models.shipping_rule import ShippingRule
from simplebilly_api.models.shipping_rule_update import ShippingRuleUpdate
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
    api_instance = simplebilly_api.ShippingRuleApi(api_client)
    rule_id = 'rule_id_example' # str | 
    shipping_rule_update = simplebilly_api.ShippingRuleUpdate() # ShippingRuleUpdate | 

    try:
        api_response = api_instance.update_shipping_rule(rule_id, shipping_rule_update)
        print("The response of ShippingRuleApi->update_shipping_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShippingRuleApi->update_shipping_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **str**|  | 
 **shipping_rule_update** | [**ShippingRuleUpdate**](ShippingRuleUpdate.md)|  | 

### Return type

[**ShippingRule**](ShippingRule.md)

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

