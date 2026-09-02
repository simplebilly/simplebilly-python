# KycRecord


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **str** | Referenz auf den Kunden/Kontakt. | [optional] 
**customer_name** | **str** | Name des Kunden (für die Suche). | [optional] 
**kyc_date** | **date** | Datum der KYC-Prüfung (GwG § 8). | [optional] 
**notes** | **str** | Freitext-Notizen. | [optional] 
**retention_until** | **date** | Aufbewahrungsfrist (GwG § 8 Abs. 4: 5 Jahre). | [optional] 
**risk_assessment** | **str** | Risikoeinschätzung (z. B. Risikoklasse). | [optional] 

## Example

```python
from simplebilly_api.models.kyc_record import KycRecord

# TODO update the JSON string below
json = "{}"
# create an instance of KycRecord from a JSON string
kyc_record_instance = KycRecord.from_json(json)
# print the JSON string representation of the object
print(KycRecord.to_json())

# convert the object into a dict
kyc_record_dict = kyc_record_instance.to_dict()
# create an instance of KycRecord from a dict
kyc_record_from_dict = KycRecord.from_dict(kyc_record_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


