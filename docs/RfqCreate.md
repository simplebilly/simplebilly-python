# RfqCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **str** |  | [optional] 
**line_items** | **object** | JSON array of &#x60;{product_id, name, sku, quantity, requested_unit_price?, quoted_unit_price?}&#x60;. | 
**notes** | **str** |  | [optional] 
**requested_date** | **date** |  | 
**response_date** | **date** |  | [optional] 
**rfq_number** | **str** |  | 
**status** | [**RfqStatus**](RfqStatus.md) | One of: draft | sent | offer_received | rejected | converted | 
**supplier_contact_id** | **str** | References the supplier entity. | [optional] 
**supplier_name** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.rfq_create import RfqCreate

# TODO update the JSON string below
json = "{}"
# create an instance of RfqCreate from a JSON string
rfq_create_instance = RfqCreate.from_json(json)
# print the JSON string representation of the object
print(RfqCreate.to_json())

# convert the object into a dict
rfq_create_dict = rfq_create_instance.to_dict()
# create an instance of RfqCreate from a dict
rfq_create_from_dict = RfqCreate.from_dict(rfq_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


