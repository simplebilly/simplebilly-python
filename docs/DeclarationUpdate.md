# DeclarationUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**declaration_type** | [**DeclarationType**](DeclarationType.md) | Art der Erklärung: \&quot;dcgk\&quot; (Entsprechenserklärung § 161 AktG) oder \&quot;unternehmensfuehrung\&quot; (Erklärung zur Unternehmensführung § 289f HGB). | [optional] 
**is_current** | **bool** | Kennzeichnet die aktuell gültige Fassung (max. eine je Mandant). | [optional] 
**text** | **str** | Inhalt der Erklärung als Markdown. | [optional] 
**valid_from** | **date** | Datum, ab dem die Erklärung gilt. | [optional] 
**version** | **str** | Versionsbezeichnung der Erklärung (z.B. \&quot;2025-01\&quot;). | [optional] 

## Example

```python
from simplebilly_api.models.declaration_update import DeclarationUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of DeclarationUpdate from a JSON string
declaration_update_instance = DeclarationUpdate.from_json(json)
# print the JSON string representation of the object
print(DeclarationUpdate.to_json())

# convert the object into a dict
declaration_update_dict = declaration_update_instance.to_dict()
# create an instance of DeclarationUpdate from a dict
declaration_update_from_dict = DeclarationUpdate.from_dict(declaration_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


