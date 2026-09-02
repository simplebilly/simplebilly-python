# DeclarationCreate


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
from simplebilly_api.models.declaration_create import DeclarationCreate

# TODO update the JSON string below
json = "{}"
# create an instance of DeclarationCreate from a JSON string
declaration_create_instance = DeclarationCreate.from_json(json)
# print the JSON string representation of the object
print(DeclarationCreate.to_json())

# convert the object into a dict
declaration_create_dict = declaration_create_instance.to_dict()
# create an instance of DeclarationCreate from a dict
declaration_create_from_dict = DeclarationCreate.from_dict(declaration_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


