# EmailTemplateUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**body** | **str** | E-mail body with optional placeholders. | [optional] 
**name** | **str** | Human-readable template name, e.g. \&quot;Follow-up after quote\&quot;. | [optional] 
**status** | [**EmailTemplateStatus**](EmailTemplateStatus.md) | One of: active | inactive | [optional] 
**subject** | **str** | E-mail subject line with optional placeholders. | [optional] 
**variables** | **object** | Placeholders used by this template, e.g. &#x60;[\&quot;contact.first_name\&quot;]&#x60;. | [optional] 

## Example

```python
from simplebilly_api.models.email_template_update import EmailTemplateUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of EmailTemplateUpdate from a JSON string
email_template_update_instance = EmailTemplateUpdate.from_json(json)
# print the JSON string representation of the object
print(EmailTemplateUpdate.to_json())

# convert the object into a dict
email_template_update_dict = email_template_update_instance.to_dict()
# create an instance of EmailTemplateUpdate from a dict
email_template_update_from_dict = EmailTemplateUpdate.from_dict(email_template_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


