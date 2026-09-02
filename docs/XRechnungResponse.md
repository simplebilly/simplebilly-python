# XRechnungResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | 
**content_type** | **str** |  | 
**filename** | **str** |  | 

## Example

```python
from simplebilly_api.models.x_rechnung_response import XRechnungResponse

# TODO update the JSON string below
json = "{}"
# create an instance of XRechnungResponse from a JSON string
x_rechnung_response_instance = XRechnungResponse.from_json(json)
# print the JSON string representation of the object
print(XRechnungResponse.to_json())

# convert the object into a dict
x_rechnung_response_dict = x_rechnung_response_instance.to_dict()
# create an instance of XRechnungResponse from a dict
x_rechnung_response_from_dict = XRechnungResponse.from_dict(x_rechnung_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


