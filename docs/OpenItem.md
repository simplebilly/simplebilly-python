# OpenItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount_due** | **str** |  | 
**amount_paid** | **str** |  | 
**customer_id** | **str** |  | [optional] 
**days_overdue** | **int** |  | [optional] 
**due_date** | **str** |  | [optional] 
**invoice_id** | **str** |  | 
**invoice_number** | **str** |  | 
**issue_date** | **str** |  | 
**open_amount** | **str** |  | 
**reminder_level** | [**ReminderLevel**](ReminderLevel.md) |  | 

## Example

```python
from simplebilly_api.models.open_item import OpenItem

# TODO update the JSON string below
json = "{}"
# create an instance of OpenItem from a JSON string
open_item_instance = OpenItem.from_json(json)
# print the JSON string representation of the object
print(OpenItem.to_json())

# convert the object into a dict
open_item_dict = open_item_instance.to_dict()
# create an instance of OpenItem from a dict
open_item_from_dict = OpenItem.from_dict(open_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


