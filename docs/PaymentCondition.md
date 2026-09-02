# PaymentCondition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**discount_days** | **int** |  | 
**discount_percentage** | **float** |  | 
**id** | **str** |  | 
**name** | **str** |  | 
**payment_term_days** | **int** |  | 

## Example

```python
from simplebilly_api.models.payment_condition import PaymentCondition

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentCondition from a JSON string
payment_condition_instance = PaymentCondition.from_json(json)
# print the JSON string representation of the object
print(PaymentCondition.to_json())

# convert the object into a dict
payment_condition_dict = payment_condition_instance.to_dict()
# create an instance of PaymentCondition from a dict
payment_condition_from_dict = PaymentCondition.from_dict(payment_condition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


