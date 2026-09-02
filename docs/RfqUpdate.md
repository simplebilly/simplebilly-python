# RfqUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **str** |  | [optional] 
**line_items** | **object** | JSON array of &#x60;{product_id, name, sku, quantity, requested_unit_price?, quoted_unit_price?}&#x60;. | [optional] 
**notes** | **str** |  | [optional] 
**requested_date** | **date** |  | [optional] 
**response_date** | **date** |  | [optional] 
**rfq_number** | **str** |  | [optional] 
**status** | [**RfqStatus**](RfqStatus.md) | One of: draft | sent | offer_received | rejected | converted | [optional] 
**supplier_contact_id** | **str** | References the supplier entity. | [optional] 
**supplier_name** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.rfq_update import RfqUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of RfqUpdate from a JSON string
rfq_update_instance = RfqUpdate.from_json(json)
# print the JSON string representation of the object
print(RfqUpdate.to_json())

# convert the object into a dict
rfq_update_dict = rfq_update_instance.to_dict()
# create an instance of RfqUpdate from a dict
rfq_update_from_dict = RfqUpdate.from_dict(rfq_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


