# ConvertResponse

Response of the proforma → invoice conversion.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoice_id** | **str** |  | 
**invoice_number** | **str** |  | 
**proforma_id** | **str** |  | 
**proforma_number** | **str** |  | 

## Example

```python
from simplebilly_api.models.convert_response import ConvertResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ConvertResponse from a JSON string
convert_response_instance = ConvertResponse.from_json(json)
# print the JSON string representation of the object
print(ConvertResponse.to_json())

# convert the object into a dict
convert_response_dict = convert_response_instance.to_dict()
# create an instance of ConvertResponse from a dict
convert_response_from_dict = ConvertResponse.from_dict(convert_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


