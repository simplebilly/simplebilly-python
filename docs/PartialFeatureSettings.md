# PartialFeatureSettings

Partial feature toggles: `None` keeps the company-type default, `Some` overrides it.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**onlineshop** | **bool** |  | [optional] 
**report_bilanz** | **bool** |  | [optional] 
**report_bwa** | **bool** |  | [optional] 
**report_euer** | **bool** |  | [optional] 
**report_gewerbesteuer** | **bool** |  | [optional] 
**report_guv** | **bool** |  | [optional] 
**report_kst** | **bool** |  | [optional] 
**report_ustva** | **bool** |  | [optional] 

## Example

```python
from simplebilly_api.models.partial_feature_settings import PartialFeatureSettings

# TODO update the JSON string below
json = "{}"
# create an instance of PartialFeatureSettings from a JSON string
partial_feature_settings_instance = PartialFeatureSettings.from_json(json)
# print the JSON string representation of the object
print(PartialFeatureSettings.to_json())

# convert the object into a dict
partial_feature_settings_dict = partial_feature_settings_instance.to_dict()
# create an instance of PartialFeatureSettings from a dict
partial_feature_settings_from_dict = PartialFeatureSettings.from_dict(partial_feature_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


