# PaymentGatewayUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config** | **object** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**gateway_type** | [**GatewayType**](GatewayType.md) |  | [optional] 
**label** | **str** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.payment_gateway_update import PaymentGatewayUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentGatewayUpdate from a JSON string
payment_gateway_update_instance = PaymentGatewayUpdate.from_json(json)
# print the JSON string representation of the object
print(PaymentGatewayUpdate.to_json())

# convert the object into a dict
payment_gateway_update_dict = payment_gateway_update_instance.to_dict()
# create an instance of PaymentGatewayUpdate from a dict
payment_gateway_update_from_dict = PaymentGatewayUpdate.from_dict(payment_gateway_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


