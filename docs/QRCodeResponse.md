# QRCodeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content_type** | **str** |  | 
**qr_code_base64** | **str** |  | 

## Example

```python
from simplebilly_api.models.qr_code_response import QRCodeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of QRCodeResponse from a JSON string
qr_code_response_instance = QRCodeResponse.from_json(json)
# print the JSON string representation of the object
print(QRCodeResponse.to_json())

# convert the object into a dict
qr_code_response_dict = qr_code_response_instance.to_dict()
# create an instance of QRCodeResponse from a dict
qr_code_response_from_dict = QRCodeResponse.from_dict(qr_code_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


