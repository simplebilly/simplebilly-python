# VatSummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**input_tax_items** | [**List[VatItem]**](VatItem.md) |  | 
**output_tax_items** | [**List[VatItem]**](VatItem.md) |  | 
**total_input_tax** | **str** |  | 
**total_output_tax** | **str** |  | 
**vat_due** | **str** |  | 

## Example

```python
from simplebilly_api.models.vat_summary import VatSummary

# TODO update the JSON string below
json = "{}"
# create an instance of VatSummary from a JSON string
vat_summary_instance = VatSummary.from_json(json)
# print the JSON string representation of the object
print(VatSummary.to_json())

# convert the object into a dict
vat_summary_dict = vat_summary_instance.to_dict()
# create an instance of VatSummary from a dict
vat_summary_from_dict = VatSummary.from_dict(vat_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


