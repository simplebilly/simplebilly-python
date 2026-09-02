# SepaDirectDebitResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content_type** | **str** |  | 
**filename** | **str** |  | 
**xml_content** | **str** |  | 

## Example

```python
from simplebilly_api.models.sepa_direct_debit_response import SepaDirectDebitResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SepaDirectDebitResponse from a JSON string
sepa_direct_debit_response_instance = SepaDirectDebitResponse.from_json(json)
# print the JSON string representation of the object
print(SepaDirectDebitResponse.to_json())

# convert the object into a dict
sepa_direct_debit_response_dict = sepa_direct_debit_response_instance.to_dict()
# create an instance of SepaDirectDebitResponse from a dict
sepa_direct_debit_response_from_dict = SepaDirectDebitResponse.from_dict(sepa_direct_debit_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


