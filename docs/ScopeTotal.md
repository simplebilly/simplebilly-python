# ScopeTotal


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**scope** | **str** |  | 
**tco2e** | **str** |  | 

## Example

```python
from simplebilly_api.models.scope_total import ScopeTotal

# TODO update the JSON string below
json = "{}"
# create an instance of ScopeTotal from a JSON string
scope_total_instance = ScopeTotal.from_json(json)
# print the JSON string representation of the object
print(ScopeTotal.to_json())

# convert the object into a dict
scope_total_dict = scope_total_instance.to_dict()
# create an instance of ScopeTotal from a dict
scope_total_from_dict = ScopeTotal.from_dict(scope_total_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


