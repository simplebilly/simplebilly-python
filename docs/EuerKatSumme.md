# EuerKatSumme


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**betrag** | **str** |  | 
**name** | **str** |  | 

## Example

```python
from simplebilly_api.models.euer_kat_summe import EuerKatSumme

# TODO update the JSON string below
json = "{}"
# create an instance of EuerKatSumme from a JSON string
euer_kat_summe_instance = EuerKatSumme.from_json(json)
# print the JSON string representation of the object
print(EuerKatSumme.to_json())

# convert the object into a dict
euer_kat_summe_dict = euer_kat_summe_instance.to_dict()
# create an instance of EuerKatSumme from a dict
euer_kat_summe_from_dict = EuerKatSumme.from_dict(euer_kat_summe_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


