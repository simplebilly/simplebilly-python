# PrintLabelResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label_url** | **str** |  | [optional] 
**message** | **str** |  | 
**sscc** | **str** |  | [optional] 
**success** | **bool** |  | 
**tracking_number** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.print_label_response import PrintLabelResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PrintLabelResponse from a JSON string
print_label_response_instance = PrintLabelResponse.from_json(json)
# print the JSON string representation of the object
print(PrintLabelResponse.to_json())

# convert the object into a dict
print_label_response_dict = print_label_response_instance.to_dict()
# create an instance of PrintLabelResponse from a dict
print_label_response_from_dict = PrintLabelResponse.from_dict(print_label_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


