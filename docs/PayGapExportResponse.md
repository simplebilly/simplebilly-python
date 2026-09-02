# PayGapExportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**csv_content** | **str** |  | 
**filename** | **str** |  | 

## Example

```python
from simplebilly_api.models.pay_gap_export_response import PayGapExportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PayGapExportResponse from a JSON string
pay_gap_export_response_instance = PayGapExportResponse.from_json(json)
# print the JSON string representation of the object
print(PayGapExportResponse.to_json())

# convert the object into a dict
pay_gap_export_response_dict = pay_gap_export_response_instance.to_dict()
# create an instance of PayGapExportResponse from a dict
pay_gap_export_response_from_dict = PayGapExportResponse.from_dict(pay_gap_export_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


