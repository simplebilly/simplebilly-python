# PrintDeliveryNoteResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | 
**pdf_url** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.print_delivery_note_response import PrintDeliveryNoteResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PrintDeliveryNoteResponse from a JSON string
print_delivery_note_response_instance = PrintDeliveryNoteResponse.from_json(json)
# print the JSON string representation of the object
print(PrintDeliveryNoteResponse.to_json())

# convert the object into a dict
print_delivery_note_response_dict = print_delivery_note_response_instance.to_dict()
# create an instance of PrintDeliveryNoteResponse from a dict
print_delivery_note_response_from_dict = PrintDeliveryNoteResponse.from_dict(print_delivery_note_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


