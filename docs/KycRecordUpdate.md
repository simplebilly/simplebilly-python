# KycRecordUpdate


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
from simplebilly_api.models.kyc_record_update import KycRecordUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of KycRecordUpdate from a JSON string
kyc_record_update_instance = KycRecordUpdate.from_json(json)
# print the JSON string representation of the object
print(KycRecordUpdate.to_json())

# convert the object into a dict
kyc_record_update_dict = kyc_record_update_instance.to_dict()
# create an instance of KycRecordUpdate from a dict
kyc_record_update_from_dict = KycRecordUpdate.from_dict(kyc_record_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


