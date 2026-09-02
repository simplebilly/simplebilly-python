# BWARevenue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**revenue_breakdown** | [**List[RevenueItem]**](RevenueItem.md) |  | 
**total_revenue** | **str** |  | 

## Example

```python
from simplebilly_api.models.bwa_revenue import BWARevenue

# TODO update the JSON string below
json = "{}"
# create an instance of BWARevenue from a JSON string
bwa_revenue_instance = BWARevenue.from_json(json)
# print the JSON string representation of the object
print(BWARevenue.to_json())

# convert the object into a dict
bwa_revenue_dict = bwa_revenue_instance.to_dict()
# create an instance of BWARevenue from a dict
bwa_revenue_from_dict = BWARevenue.from_dict(bwa_revenue_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


