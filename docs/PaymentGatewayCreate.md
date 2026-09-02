# PaymentGatewayCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config** | **object** |  | 
**created_at** | **datetime** |  | 
**deleted_at** | **datetime** |  | [optional] 
**enabled** | **bool** |  | 
**gateway_type** | [**GatewayType**](GatewayType.md) |  | 
**label** | **str** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.payment_gateway_create import PaymentGatewayCreate

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentGatewayCreate from a JSON string
payment_gateway_create_instance = PaymentGatewayCreate.from_json(json)
# print the JSON string representation of the object
print(PaymentGatewayCreate.to_json())

# convert the object into a dict
payment_gateway_create_dict = payment_gateway_create_instance.to_dict()
# create an instance of PaymentGatewayCreate from a dict
payment_gateway_create_from_dict = PaymentGatewayCreate.from_dict(payment_gateway_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


