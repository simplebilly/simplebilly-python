# ShareholderCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **str** | Anschrift des Aktionärs (§ 67 Abs. 1 AktG). | [optional] 
**birth_date** | **date** | Geburtsdatum des Aktionärs (§ 67 Abs. 1 AktG). | [optional] 
**email** | **str** | Elektronische Adresse (E-Mail) für die Kommunikation der Gesellschaft. | [optional] 
**first_name** | **str** | Vorname des Aktionärs (§ 67 Abs. 1 AktG). | [optional] 
**last_name** | **str** | Nachname des Aktionärs (§ 67 Abs. 1 AktG). | [optional] 
**share_number** | **str** | Aktiennummer bzw. Sammelurkunde (bei Nennbetragsaktien). | [optional] 
**shares** | **str** | Stückzahl der gehaltenen Stückaktien (§ 67 Abs. 1 AktG). | [optional] 

## Example

```python
from simplebilly_api.models.shareholder_create import ShareholderCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ShareholderCreate from a JSON string
shareholder_create_instance = ShareholderCreate.from_json(json)
# print the JSON string representation of the object
print(ShareholderCreate.to_json())

# convert the object into a dict
shareholder_create_dict = shareholder_create_instance.to_dict()
# create an instance of ShareholderCreate from a dict
shareholder_create_from_dict = ShareholderCreate.from_dict(shareholder_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


