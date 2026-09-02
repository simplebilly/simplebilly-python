# TaxRateCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**country_code** | **str** | ISO 3166-1 alpha-2 country code. | 
**effective_from** | **date** | Date this rate took effect; &#x60;None&#x60; &#x3D; not date-bound. | [optional] 
**is_default** | **bool** | Default rate for the country (one per country); fallback for lookups when no dated rate applies. | 
**name** | **str** | Human name, e.g. \&quot;VAT\&quot;. | 
**rate_percent** | **int** | Rate in hundredths of a percent: 1900 &#x3D; 19.00%. | 

## Example

```python
from simplebilly_api.models.tax_rate_create import TaxRateCreate

# TODO update the JSON string below
json = "{}"
# create an instance of TaxRateCreate from a JSON string
tax_rate_create_instance = TaxRateCreate.from_json(json)
# print the JSON string representation of the object
print(TaxRateCreate.to_json())

# convert the object into a dict
tax_rate_create_dict = tax_rate_create_instance.to_dict()
# create an instance of TaxRateCreate from a dict
tax_rate_create_from_dict = TaxRateCreate.from_dict(tax_rate_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


