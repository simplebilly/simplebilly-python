# UmsatzsteuerReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**generated_at** | **str** |  | 
**input_tax** | [**List[VatDetail]**](VatDetail.md) |  | 
**output_tax** | [**List[VatDetail]**](VatDetail.md) |  | 
**period** | **str** |  | 
**total_input_tax** | **str** |  | 
**total_output_tax** | **str** |  | 
**vat_payable** | **str** |  | 
**vat_refund** | **str** |  | 

## Example

```python
from simplebilly_api.models.umsatzsteuer_report import UmsatzsteuerReport

# TODO update the JSON string below
json = "{}"
# create an instance of UmsatzsteuerReport from a JSON string
umsatzsteuer_report_instance = UmsatzsteuerReport.from_json(json)
# print the JSON string representation of the object
print(UmsatzsteuerReport.to_json())

# convert the object into a dict
umsatzsteuer_report_dict = umsatzsteuer_report_instance.to_dict()
# create an instance of UmsatzsteuerReport from a dict
umsatzsteuer_report_from_dict = UmsatzsteuerReport.from_dict(umsatzsteuer_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


