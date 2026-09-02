# VatDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count** | **int** |  | 
**net_amount** | **str** |  | 
**tax_amount** | **str** |  | 
**tax_rate** | **str** |  | 

## Example

```python
from simplebilly_api.models.vat_detail import VatDetail

# TODO update the JSON string below
json = "{}"
# create an instance of VatDetail from a JSON string
vat_detail_instance = VatDetail.from_json(json)
# print the JSON string representation of the object
print(VatDetail.to_json())

# convert the object into a dict
vat_detail_dict = vat_detail_instance.to_dict()
# create an instance of VatDetail from a dict
vat_detail_from_dict = VatDetail.from_dict(vat_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


