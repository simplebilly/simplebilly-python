# HrTrainingOverview


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assigned_count** | **int** |  | 
**code** | **str** |  | 
**completed_count** | **int** |  | 
**overdue_count** | **int** |  | 
**title** | **str** |  | 
**training_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.hr_training_overview import HrTrainingOverview

# TODO update the JSON string below
json = "{}"
# create an instance of HrTrainingOverview from a JSON string
hr_training_overview_instance = HrTrainingOverview.from_json(json)
# print the JSON string representation of the object
print(HrTrainingOverview.to_json())

# convert the object into a dict
hr_training_overview_dict = hr_training_overview_instance.to_dict()
# create an instance of HrTrainingOverview from a dict
hr_training_overview_from_dict = HrTrainingOverview.from_dict(hr_training_overview_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


