# CreateShipmentRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**carrier** | **str** | Carrier name as configured in shipping settings: &#x60;ups&#x60; or &#x60;dhl&#x60;. | 
**service** | **str** |  | [optional] 
**weight_kg** | **float** |  | [optional] 

## Example

```python
from simplebilly_api.models.create_shipment_request import CreateShipmentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipmentRequest from a JSON string
create_shipment_request_instance = CreateShipmentRequest.from_json(json)
# print the JSON string representation of the object
print(CreateShipmentRequest.to_json())

# convert the object into a dict
create_shipment_request_dict = create_shipment_request_instance.to_dict()
# create an instance of CreateShipmentRequest from a dict
create_shipment_request_from_dict = CreateShipmentRequest.from_dict(create_shipment_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


