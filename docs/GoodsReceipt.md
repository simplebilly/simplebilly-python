# GoodsReceipt


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gr_number** | **str** |  | 
**line_items** | **object** | JSON array of &#x60;{product_id, name, quantity, batch_number?, expiry_date?, bin_location?}&#x60;. | 
**notes** | **str** |  | [optional] 
**purchase_order_id** | **str** | References the purchase order entity. | [optional] 
**receipt_date** | **date** |  | 
**supplier_contact_id** | **str** | References the supplier entity. | [optional] 
**supplier_name** | **str** |  | [optional] 
**warehouse_id** | **str** | References the warehouse entity. | 

## Example

```python
from simplebilly_api.models.goods_receipt import GoodsReceipt

# TODO update the JSON string below
json = "{}"
# create an instance of GoodsReceipt from a JSON string
goods_receipt_instance = GoodsReceipt.from_json(json)
# print the JSON string representation of the object
print(GoodsReceipt.to_json())

# convert the object into a dict
goods_receipt_dict = goods_receipt_instance.to_dict()
# create an instance of GoodsReceipt from a dict
goods_receipt_from_dict = GoodsReceipt.from_dict(goods_receipt_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


