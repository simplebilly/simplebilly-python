# PeppolResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | 
**content_type** | **str** |  | 
**filename** | **str** |  | 

## Example

```python
from simplebilly_api.models.peppol_response import PeppolResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PeppolResponse from a JSON string
peppol_response_instance = PeppolResponse.from_json(json)
# print the JSON string representation of the object
print(PeppolResponse.to_json())

# convert the object into a dict
peppol_response_dict = peppol_response_instance.to_dict()
# create an instance of PeppolResponse from a dict
peppol_response_from_dict = PeppolResponse.from_dict(peppol_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


