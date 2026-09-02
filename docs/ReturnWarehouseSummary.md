# ReturnWarehouseSummary

Aggregation for a single warehouse.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items_restocked** | **int** |  | 
**items_scrapped** | **int** |  | 
**returns** | **int** |  | 
**warehouse_id** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.return_warehouse_summary import ReturnWarehouseSummary

# TODO update the JSON string below
json = "{}"
# create an instance of ReturnWarehouseSummary from a JSON string
return_warehouse_summary_instance = ReturnWarehouseSummary.from_json(json)
# print the JSON string representation of the object
print(ReturnWarehouseSummary.to_json())

# convert the object into a dict
return_warehouse_summary_dict = return_warehouse_summary_instance.to_dict()
# create an instance of ReturnWarehouseSummary from a dict
return_warehouse_summary_from_dict = ReturnWarehouseSummary.from_dict(return_warehouse_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


