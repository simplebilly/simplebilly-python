# DatevImportRow


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | **str** |  | 
**amount** | **str** |  | 
**base_amount** | **str** |  | 
**base_currency** | **str** |  | 
**booking_text** | **str** |  | 
**bu_key** | **str** |  | 
**cost_center1** | **str** |  | 
**cost_center2** | **str** |  | 
**currency** | **str** |  | 
**debit_credit** | **str** |  | 
**discount** | **str** |  | 
**document_date** | **str** |  | 
**document_field2** | **str** |  | 
**document_number** | **str** |  | 
**eu_country_vat_id** | **str** |  | 
**eu_tax_rate** | **str** |  | 
**exchange_rate** | **str** |  | 
**opposite_account** | **str** |  | 

## Example

```python
from simplebilly_api.models.datev_import_row import DatevImportRow

# TODO update the JSON string below
json = "{}"
# create an instance of DatevImportRow from a JSON string
datev_import_row_instance = DatevImportRow.from_json(json)
# print the JSON string representation of the object
print(DatevImportRow.to_json())

# convert the object into a dict
datev_import_row_dict = datev_import_row_instance.to_dict()
# create an instance of DatevImportRow from a dict
datev_import_row_from_dict = DatevImportRow.from_dict(datev_import_row_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


