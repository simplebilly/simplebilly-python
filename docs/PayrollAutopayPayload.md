# PayrollAutopayPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**debtor_bic** | **str** |  | [optional] 
**debtor_iban** | **str** |  | [optional] 
**debtor_name** | **str** |  | [optional] 
**execution_date** | **date** |  | [optional] 

## Example

```python
from simplebilly_api.models.payroll_autopay_payload import PayrollAutopayPayload

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollAutopayPayload from a JSON string
payroll_autopay_payload_instance = PayrollAutopayPayload.from_json(json)
# print the JSON string representation of the object
print(PayrollAutopayPayload.to_json())

# convert the object into a dict
payroll_autopay_payload_dict = payroll_autopay_payload_instance.to_dict()
# create an instance of PayrollAutopayPayload from a dict
payroll_autopay_payload_from_dict = PayrollAutopayPayload.from_dict(payroll_autopay_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


