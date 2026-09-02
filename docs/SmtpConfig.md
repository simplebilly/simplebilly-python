# SmtpConfig


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**encryption** | [**SmtpEncryption**](SmtpEncryption.md) |  | 
**from_address** | **str** |  | 
**from_name** | **str** |  | [optional] 
**host** | **str** |  | 
**password** | **str** |  | 
**port** | **int** |  | 
**timeout_seconds** | **int** |  | [optional] 
**username** | **str** |  | 

## Example

```python
from simplebilly_api.models.smtp_config import SmtpConfig

# TODO update the JSON string below
json = "{}"
# create an instance of SmtpConfig from a JSON string
smtp_config_instance = SmtpConfig.from_json(json)
# print the JSON string representation of the object
print(SmtpConfig.to_json())

# convert the object into a dict
smtp_config_dict = smtp_config_instance.to_dict()
# create an instance of SmtpConfig from a dict
smtp_config_from_dict = SmtpConfig.from_dict(smtp_config_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


