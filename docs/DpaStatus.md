# DpaStatus

DPA acceptance status of the tenant.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accepted** | **bool** |  | 
**accepted_at** | **str** |  | [optional] 
**accepted_by** | **str** |  | [optional] 
**version** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.dpa_status import DpaStatus

# TODO update the JSON string below
json = "{}"
# create an instance of DpaStatus from a JSON string
dpa_status_instance = DpaStatus.from_json(json)
# print the JSON string representation of the object
print(DpaStatus.to_json())

# convert the object into a dict
dpa_status_dict = dpa_status_instance.to_dict()
# create an instance of DpaStatus from a dict
dpa_status_from_dict = DpaStatus.from_dict(dpa_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


