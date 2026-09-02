# RateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer** | [**CustomerInfo**](CustomerInfo.md) |  | [optional] 
**packages** | [**List[Package]**](Package.md) |  | 
**recipient** | [**Address**](Address.md) |  | 
**sender** | [**Address**](Address.md) |  | 

## Example

```python
from simplebilly_api.models.rate_request import RateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RateRequest from a JSON string
rate_request_instance = RateRequest.from_json(json)
# print the JSON string representation of the object
print(RateRequest.to_json())

# convert the object into a dict
rate_request_dict = rate_request_instance.to_dict()
# create an instance of RateRequest from a dict
rate_request_from_dict = RateRequest.from_dict(rate_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


