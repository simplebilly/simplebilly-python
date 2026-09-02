# SilentPartner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contract_date** | **date** | Datum des Vertragsabschlusses. | [optional] 
**einlage** | **str** | Einlage (§ 230 HGB). | [optional] 
**gewinnquote_pct** | **str** | Gewinnbeteiligungsquote in Prozent (§ 231 HGB). | [optional] 
**gewinnvortrag** | **str** | Nicht erhobene Gewinne (§ 232 Abs. 3 HGB). | [optional] 
**instrument_type** | [**InstrumentType**](InstrumentType.md) | Instrument: \&quot;typisch\&quot; | \&quot;atypisch\&quot; | \&quot;partiarisches_darlehen\&quot; | \&quot;genussrecht\&quot;. | 
**kest_pflichtig** | **bool** | 25 % Kapitalertragsteuer einbehalten (§ 43 Abs. 1 Nr. 3 EStG; typisch + partiarisches Darlehen). | [optional] 
**name** | **str** | Name des stillen Gesellschafters. | [optional] 
**notes** | **str** | Freitext-Notizen. | [optional] 
**verlust_verrechnungskonto** | **str** | Kumulierte Verluste gegen die Einlage (§ 232 Abs. 2 HGB, ≤ Einlage). | [optional] 
**verlustbeteiligung** | **bool** | Verlustbeteiligung (§ 231 Abs. 2 HGB; kann ausgeschlossen werden). | [optional] 

## Example

```python
from simplebilly_api.models.silent_partner import SilentPartner

# TODO update the JSON string below
json = "{}"
# create an instance of SilentPartner from a JSON string
silent_partner_instance = SilentPartner.from_json(json)
# print the JSON string representation of the object
print(SilentPartner.to_json())

# convert the object into a dict
silent_partner_dict = silent_partner_instance.to_dict()
# create an instance of SilentPartner from a dict
silent_partner_from_dict = SilentPartner.from_dict(silent_partner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


