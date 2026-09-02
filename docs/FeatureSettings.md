# FeatureSettings

Feature toggles for a tenant.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**onlineshop** | **bool** | Online shop / storefront module (default: enabled). | 
**report_bilanz** | **bool** | Bilanz (balance sheet) report. | 
**report_bwa** | **bool** | BWA (betriebswirtschaftliche Auswertung). | 
**report_euer** | **bool** | EÜR (Einnahmen-Überschuss-Rechnung). | 
**report_gewerbesteuer** | **bool** | Gewerbesteuer report. | 
**report_guv** | **bool** | GuV (profit &amp; loss) report. | 
**report_kst** | **bool** | KSt (Körperschaftsteuer) report. | 
**report_ustva** | **bool** | UStVA (Umsatzsteuervoranmeldung). | 

## Example

```python
from simplebilly_api.models.feature_settings import FeatureSettings

# TODO update the JSON string below
json = "{}"
# create an instance of FeatureSettings from a JSON string
feature_settings_instance = FeatureSettings.from_json(json)
# print the JSON string representation of the object
print(FeatureSettings.to_json())

# convert the object into a dict
feature_settings_dict = feature_settings_instance.to_dict()
# create an instance of FeatureSettings from a dict
feature_settings_from_dict = FeatureSettings.from_dict(feature_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


