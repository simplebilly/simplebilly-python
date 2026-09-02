# PayrollPayPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**payment_date** | **date** |  | 

## Example

```python
from simplebilly_api.models.payroll_pay_payload import PayrollPayPayload

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollPayPayload from a JSON string
payroll_pay_payload_instance = PayrollPayPayload.from_json(json)
# print the JSON string representation of the object
print(PayrollPayPayload.to_json())

# convert the object into a dict
payroll_pay_payload_dict = payroll_pay_payload_instance.to_dict()
# create an instance of PayrollPayPayload from a dict
payroll_pay_payload_from_dict = PayrollPayPayload.from_dict(payroll_pay_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


