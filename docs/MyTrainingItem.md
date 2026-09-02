# MyTrainingItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assignment_id** | **UUID** |  | 
**certificate_id** | **str** |  | [optional] 
**code** | **str** |  | 
**description** | **str** |  | [optional] 
**due_date** | **date** |  | [optional] 
**last_score** | **int** |  | [optional] 
**pass_score** | **int** |  | 
**passed** | **bool** |  | [optional] 
**status** | [**AssignmentStatus**](AssignmentStatus.md) |  | 
**title** | **str** |  | 
**training_id** | **UUID** |  | 
**valid_until** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.my_training_item import MyTrainingItem

# TODO update the JSON string below
json = "{}"
# create an instance of MyTrainingItem from a JSON string
my_training_item_instance = MyTrainingItem.from_json(json)
# print the JSON string representation of the object
print(MyTrainingItem.to_json())

# convert the object into a dict
my_training_item_dict = my_training_item_instance.to_dict()
# create an instance of MyTrainingItem from a dict
my_training_item_from_dict = MyTrainingItem.from_dict(my_training_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


