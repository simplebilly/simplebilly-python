# InstituteStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**checklist** | [**List[InstituteCheckItem]**](InstituteCheckItem.md) |  | 
**deadlines** | [**InstituteDeadlines**](InstituteDeadlines.md) |  | 
**institute_type** | **str** |  | 
**kapitalmarktorientiert** | **bool** |  | 

## Example

```python
from simplebilly_api.models.institute_status import InstituteStatus

# TODO update the JSON string below
json = "{}"
# create an instance of InstituteStatus from a JSON string
institute_status_instance = InstituteStatus.from_json(json)
# print the JSON string representation of the object
print(InstituteStatus.to_json())

# convert the object into a dict
institute_status_dict = institute_status_instance.to_dict()
# create an instance of InstituteStatus from a dict
institute_status_from_dict = InstituteStatus.from_dict(institute_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


