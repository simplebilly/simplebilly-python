# StillePartnerZeile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**auseinandersetzungsguthaben** | **str** |  | 
**gewinnanteil** | **str** |  | 
**gewinnvortrag** | **str** |  | 
**hinweis** | **str** |  | [optional] 
**instrument_type** | **str** |  | 
**kest** | **str** |  | 
**name** | **str** |  | 
**verlust_verrechnungskonto** | **str** |  | 
**verlustanteil** | **str** |  | 

## Example

```python
from simplebilly_api.models.stille_partner_zeile import StillePartnerZeile

# TODO update the JSON string below
json = "{}"
# create an instance of StillePartnerZeile from a JSON string
stille_partner_zeile_instance = StillePartnerZeile.from_json(json)
# print the JSON string representation of the object
print(StillePartnerZeile.to_json())

# convert the object into a dict
stille_partner_zeile_dict = stille_partner_zeile_instance.to_dict()
# create an instance of StillePartnerZeile from a dict
stille_partner_zeile_from_dict = StillePartnerZeile.from_dict(stille_partner_zeile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


