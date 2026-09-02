# PaymentGateway


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config** | **object** |  | 
**created_at** | **datetime** |  | 
**deleted_at** | **datetime** |  | [optional] 
**enabled** | **bool** |  | 
**gateway_id** | **str** |  | 
**gateway_type** | [**GatewayType**](GatewayType.md) |  | 
**label** | **str** |  | 
**tenant_id** | **UUID** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.payment_gateway import PaymentGateway

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentGateway from a JSON string
payment_gateway_instance = PaymentGateway.from_json(json)
# print the JSON string representation of the object
print(PaymentGateway.to_json())

# convert the object into a dict
payment_gateway_dict = payment_gateway_instance.to_dict()
# create an instance of PaymentGateway from a dict
payment_gateway_from_dict = PaymentGateway.from_dict(payment_gateway_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


