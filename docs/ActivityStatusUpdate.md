# ActivityStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.activity_status_update import ActivityStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ActivityStatusUpdate from a JSON string
activity_status_update_instance = ActivityStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(ActivityStatusUpdate.to_json())

# convert the object into a dict
activity_status_update_dict = activity_status_update_instance.to_dict()
# create an instance of ActivityStatusUpdate from a dict
activity_status_update_from_dict = ActivityStatusUpdate.from_dict(activity_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


