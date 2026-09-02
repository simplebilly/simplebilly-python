# KonzernBeteiligung


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**company_name** | **str** |  | 
**control_basis** | **List[str]** | Erfüllte Kontroll-Indikatoren (§ 290 Abs. 2 HGB) als deutsche Bezeichnungen. | 
**controlled** | **bool** |  | 
**ownership_pct** | **str** |  | 

## Example

```python
from simplebilly_api.models.konzern_beteiligung import KonzernBeteiligung

# TODO update the JSON string below
json = "{}"
# create an instance of KonzernBeteiligung from a JSON string
konzern_beteiligung_instance = KonzernBeteiligung.from_json(json)
# print the JSON string representation of the object
print(KonzernBeteiligung.to_json())

# convert the object into a dict
konzern_beteiligung_dict = konzern_beteiligung_instance.to_dict()
# create an instance of KonzernBeteiligung from a dict
konzern_beteiligung_from_dict = KonzernBeteiligung.from_dict(konzern_beteiligung_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


