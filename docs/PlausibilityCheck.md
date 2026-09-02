# PlausibilityCheck


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**detail** | **str** |  | 
**id** | **str** |  | 
**name** | **str** |  | 
**severity** | [**Severity**](Severity.md) |  | 
**status** | [**CheckStatus**](CheckStatus.md) |  | 

## Example

```python
from simplebilly_api.models.plausibility_check import PlausibilityCheck

# TODO update the JSON string below
json = "{}"
# create an instance of PlausibilityCheck from a JSON string
plausibility_check_instance = PlausibilityCheck.from_json(json)
# print the JSON string representation of the object
print(PlausibilityCheck.to_json())

# convert the object into a dict
plausibility_check_dict = plausibility_check_instance.to_dict()
# create an instance of PlausibilityCheck from a dict
plausibility_check_from_dict = PlausibilityCheck.from_dict(plausibility_check_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


