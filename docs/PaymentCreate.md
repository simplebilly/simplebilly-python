# PaymentCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **str** |  | [optional] 
**attachment** | **object** |  | [optional] 
**currency** | **str** |  | [optional] 
**customer_id** | **str** | References the customer entity. | [optional] 
**description** | **str** |  | [optional] 
**metadata** | **object** |  | [optional] 
**method** | [**PaymentMethod**](PaymentMethod.md) |  | [optional] 
**payment_date** | **datetime** |  | [optional] 
**reference** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.payment_create import PaymentCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentCreate from a JSON string
payment_create_instance = PaymentCreate.from_json(json)
# print the JSON string representation of the object
print(PaymentCreate.to_json())

# convert the object into a dict
payment_create_dict = payment_create_instance.to_dict()
# create an instance of PaymentCreate from a dict
payment_create_from_dict = PaymentCreate.from_dict(payment_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


