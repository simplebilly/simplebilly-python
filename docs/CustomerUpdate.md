# CustomerUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address** | **object** |  | [optional] 
**contact_person** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**external_order_number** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**payment_grace_period_days** | **int** |  | [optional] 
**phone** | **str** |  | [optional] 
**vat_id** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.customer_update import CustomerUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerUpdate from a JSON string
customer_update_instance = CustomerUpdate.from_json(json)
# print the JSON string representation of the object
print(CustomerUpdate.to_json())

# convert the object into a dict
customer_update_dict = customer_update_instance.to_dict()
# create an instance of CustomerUpdate from a dict
customer_update_from_dict = CustomerUpdate.from_dict(customer_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


