# PayrollCreatePayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**employee_ids** | **List[UUID]** |  | 
**extra_payments** | [**List[ExtraPayment]**](ExtraPayment.md) |  | [optional] 
**month** | **int** |  | 
**year** | **int** |  | 

## Example

```python
from simplebilly_api.models.payroll_create_payload import PayrollCreatePayload

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollCreatePayload from a JSON string
payroll_create_payload_instance = PayrollCreatePayload.from_json(json)
# print the JSON string representation of the object
print(PayrollCreatePayload.to_json())

# convert the object into a dict
payroll_create_payload_dict = payroll_create_payload_instance.to_dict()
# create an instance of PayrollCreatePayload from a dict
payroll_create_payload_from_dict = PayrollCreatePayload.from_dict(payroll_create_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


