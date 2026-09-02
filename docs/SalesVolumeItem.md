# SalesVolumeItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **str** |  | 
**contact_type** | **str** |  | 
**last_purchase_date** | **str** |  | [optional] 
**name** | **str** |  | 
**total_invoices** | **int** |  | 
**total_revenue** | **str** |  | 

## Example

```python
from simplebilly_api.models.sales_volume_item import SalesVolumeItem

# TODO update the JSON string below
json = "{}"
# create an instance of SalesVolumeItem from a JSON string
sales_volume_item_instance = SalesVolumeItem.from_json(json)
# print the JSON string representation of the object
print(SalesVolumeItem.to_json())

# convert the object into a dict
sales_volume_item_dict = sales_volume_item_instance.to_dict()
# create an instance of SalesVolumeItem from a dict
sales_volume_item_from_dict = SalesVolumeItem.from_dict(sales_volume_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


