# ExtraPayment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** |  | 
**employee_id** | **UUID** |  | 
**reason** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.extra_payment import ExtraPayment

# TODO update the JSON string below
json = "{}"
# create an instance of ExtraPayment from a JSON string
extra_payment_instance = ExtraPayment.from_json(json)
# print the JSON string representation of the object
print(ExtraPayment.to_json())

# convert the object into a dict
extra_payment_dict = extra_payment_instance.to_dict()
# create an instance of ExtraPayment from a dict
extra_payment_from_dict = ExtraPayment.from_dict(extra_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


