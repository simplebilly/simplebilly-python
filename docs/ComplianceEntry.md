# ComplianceEntry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | 
**module** | **str** |  | 
**regulations** | **List[str]** |  | 

## Example

```python
from simplebilly_api.models.compliance_entry import ComplianceEntry

# TODO update the JSON string below
json = "{}"
# create an instance of ComplianceEntry from a JSON string
compliance_entry_instance = ComplianceEntry.from_json(json)
# print the JSON string representation of the object
print(ComplianceEntry.to_json())

# convert the object into a dict
compliance_entry_dict = compliance_entry_instance.to_dict()
# create an instance of ComplianceEntry from a dict
compliance_entry_from_dict = ComplianceEntry.from_dict(compliance_entry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


