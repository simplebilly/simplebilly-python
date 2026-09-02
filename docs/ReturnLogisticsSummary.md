# ReturnLogisticsSummary

Warehouse-level aggregation for the returns logistics dashboard.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**by_status** | **object** | Number of return orders per status. | 
**by_warehouse** | [**List[ReturnWarehouseSummary]**](ReturnWarehouseSummary.md) | Per-warehouse aggregation. | 
**items_restocked** | **int** | Sum of &#x60;restock: true&#x60; line-item quantities. | 
**items_scrapped** | **int** | Sum of &#x60;restock: false&#x60; line-item quantities (scrapped/disposed). | 
**total_items** | **int** | Sum of all line-item quantities across returns. | 
**total_returns** | **int** | Total number of return orders (excluding soft-deleted). | 

## Example

```python
from simplebilly_api.models.return_logistics_summary import ReturnLogisticsSummary

# TODO update the JSON string below
json = "{}"
# create an instance of ReturnLogisticsSummary from a JSON string
return_logistics_summary_instance = ReturnLogisticsSummary.from_json(json)
# print the JSON string representation of the object
print(ReturnLogisticsSummary.to_json())

# convert the object into a dict
return_logistics_summary_dict = return_logistics_summary_instance.to_dict()
# create an instance of ReturnLogisticsSummary from a dict
return_logistics_summary_from_dict = ReturnLogisticsSummary.from_dict(return_logistics_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


