# AllocatePaymentRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **float** |  | 
**invoice_id** | **str** |  | 
**payment_id** | **UUID** |  | 

## Example

```python
from simplebilly_api.models.allocate_payment_request import AllocatePaymentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AllocatePaymentRequest from a JSON string
allocate_payment_request_instance = AllocatePaymentRequest.from_json(json)
# print the JSON string representation of the object
print(AllocatePaymentRequest.to_json())

# convert the object into a dict
allocate_payment_request_dict = allocate_payment_request_instance.to_dict()
# create an instance of AllocatePaymentRequest from a dict
allocate_payment_request_from_dict = AllocatePaymentRequest.from_dict(allocate_payment_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


