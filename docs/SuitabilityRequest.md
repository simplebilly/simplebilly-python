# SuitabilityRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_annual_volume** | **int** |  | [optional] 
**items** | [**List[CartItemInput]**](CartItemInput.md) |  | 
**recipient** | [**Address**](Address.md) |  | 
**sender** | [**Address**](Address.md) |  | 

## Example

```python
from simplebilly_api.models.suitability_request import SuitabilityRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SuitabilityRequest from a JSON string
suitability_request_instance = SuitabilityRequest.from_json(json)
# print the JSON string representation of the object
print(SuitabilityRequest.to_json())

# convert the object into a dict
suitability_request_dict = suitability_request_instance.to_dict()
# create an instance of SuitabilityRequest from a dict
suitability_request_from_dict = SuitabilityRequest.from_dict(suitability_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


