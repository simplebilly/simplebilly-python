# UsageSnapshot

Current usage for a tenant. `overage_seats` is what billing charges 5€/seat/month on.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connectors** | **int** |  | 
**invoices_this_month** | **int** |  | 
**overage_seats** | **int** |  | 
**users** | **int** |  | 

## Example

```python
from simplebilly_api.models.usage_snapshot import UsageSnapshot

# TODO update the JSON string below
json = "{}"
# create an instance of UsageSnapshot from a JSON string
usage_snapshot_instance = UsageSnapshot.from_json(json)
# print the JSON string representation of the object
print(UsageSnapshot.to_json())

# convert the object into a dict
usage_snapshot_dict = usage_snapshot_instance.to_dict()
# create an instance of UsageSnapshot from a dict
usage_snapshot_from_dict = UsageSnapshot.from_dict(usage_snapshot_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


