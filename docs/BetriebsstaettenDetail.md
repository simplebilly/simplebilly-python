# BetriebsstaettenDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**beschaefigte** | **int** |  | 
**monatlicher_beitrag** | **str** |  | 
**name** | **str** |  | 

## Example

```python
from simplebilly_api.models.betriebsstaetten_detail import BetriebsstaettenDetail

# TODO update the JSON string below
json = "{}"
# create an instance of BetriebsstaettenDetail from a JSON string
betriebsstaetten_detail_instance = BetriebsstaettenDetail.from_json(json)
# print the JSON string representation of the object
print(BetriebsstaettenDetail.to_json())

# convert the object into a dict
betriebsstaetten_detail_dict = betriebsstaetten_detail_instance.to_dict()
# create an instance of BetriebsstaettenDetail from a dict
betriebsstaetten_detail_from_dict = BetriebsstaettenDetail.from_dict(betriebsstaetten_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


