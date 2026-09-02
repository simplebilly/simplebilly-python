# EmailTemplate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**body** | **str** | E-mail body with optional placeholders. | 
**name** | **str** | Human-readable template name, e.g. \&quot;Follow-up after quote\&quot;. | 
**status** | [**EmailTemplateStatus**](EmailTemplateStatus.md) | One of: active | inactive | 
**subject** | **str** | E-mail subject line with optional placeholders. | 
**variables** | **object** | Placeholders used by this template, e.g. &#x60;[\&quot;contact.first_name\&quot;]&#x60;. | [optional] 

## Example

```python
from simplebilly_api.models.email_template import EmailTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of EmailTemplate from a JSON string
email_template_instance = EmailTemplate.from_json(json)
# print the JSON string representation of the object
print(EmailTemplate.to_json())

# convert the object into a dict
email_template_dict = email_template_instance.to_dict()
# create an instance of EmailTemplate from a dict
email_template_from_dict = EmailTemplate.from_dict(email_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


