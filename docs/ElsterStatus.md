# ElsterStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cert_configured** | **bool** |  | 
**eric_available** | **bool** |  | 
**eric_version** | **str** |  | [optional] 
**feature_enabled** | **bool** |  | 
**hint** | **str** |  | 
**mode** | **str** |  | 
**vendor_id_configured** | **bool** |  | 

## Example

```python
from simplebilly_api.models.elster_status import ElsterStatus

# TODO update the JSON string below
json = "{}"
# create an instance of ElsterStatus from a JSON string
elster_status_instance = ElsterStatus.from_json(json)
# print the JSON string representation of the object
print(ElsterStatus.to_json())

# convert the object into a dict
elster_status_dict = elster_status_instance.to_dict()
# create an instance of ElsterStatus from a dict
elster_status_from_dict = ElsterStatus.from_dict(elster_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


