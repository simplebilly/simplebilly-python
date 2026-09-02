# BankLookup


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bank_name** | **str** |  | [optional] 
**bic** | **str** |  | [optional] 
**iban** | **str** |  | 
**nextgenpsd2_url** | **str** |  | [optional] 
**psd2_supported** | **bool** |  | 

## Example

```python
from simplebilly_api.models.bank_lookup import BankLookup

# TODO update the JSON string below
json = "{}"
# create an instance of BankLookup from a JSON string
bank_lookup_instance = BankLookup.from_json(json)
# print the JSON string representation of the object
print(BankLookup.to_json())

# convert the object into a dict
bank_lookup_dict = bank_lookup_instance.to_dict()
# create an instance of BankLookup from a dict
bank_lookup_from_dict = BankLookup.from_dict(bank_lookup_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


