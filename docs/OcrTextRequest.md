# OcrTextRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ocr_text** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.ocr_text_request import OcrTextRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OcrTextRequest from a JSON string
ocr_text_request_instance = OcrTextRequest.from_json(json)
# print the JSON string representation of the object
print(OcrTextRequest.to_json())

# convert the object into a dict
ocr_text_request_dict = ocr_text_request_instance.to_dict()
# create an instance of OcrTextRequest from a dict
ocr_text_request_from_dict = OcrTextRequest.from_dict(ocr_text_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


