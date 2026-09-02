# CustomerGroup


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**member_ids** | **List[str]** | Contact ids that are members of this group. | [optional] 
**membership_filter** | **str** | Rule description for membership, e.g. \&quot;orders &gt; 5 last 12 months\&quot;. | [optional] 
**name** | **str** | Unique group name, e.g. \&quot;VIP\&quot;, \&quot;Wholesale\&quot;, \&quot;Newsletter\&quot;. | 

## Example

```python
from simplebilly_api.models.customer_group import CustomerGroup

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerGroup from a JSON string
customer_group_instance = CustomerGroup.from_json(json)
# print the JSON string representation of the object
print(CustomerGroup.to_json())

# convert the object into a dict
customer_group_dict = customer_group_instance.to_dict()
# create an instance of CustomerGroup from a dict
customer_group_from_dict = CustomerGroup.from_dict(customer_group_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


