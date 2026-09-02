# BWASummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gross_profit** | **str** |  | 
**net_profit** | **str** |  | 
**open_invoices_count** | **int** |  | 
**open_invoices_total** | **str** |  | 
**overdue_invoices_count** | **int** |  | 
**overdue_invoices_total** | **str** |  | 
**profit_margin** | **float** |  | 

## Example

```python
from simplebilly_api.models.bwa_summary import BWASummary

# TODO update the JSON string below
json = "{}"
# create an instance of BWASummary from a JSON string
bwa_summary_instance = BWASummary.from_json(json)
# print the JSON string representation of the object
print(BWASummary.to_json())

# convert the object into a dict
bwa_summary_dict = bwa_summary_instance.to_dict()
# create an instance of BWASummary from a dict
bwa_summary_from_dict = BWASummary.from_dict(bwa_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


