# ProductUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**availability** | **str** |  | [optional] 
**barcode** | **str** |  | [optional] 
**brand** | **str** |  | [optional] 
**category_id** | **str** |  | [optional] 
**condition** | **str** |  | [optional] 
**default_ledger_account** | **str** |  | [optional] 
**default_price** | **str** |  | [optional] 
**default_price_formula_id** | **UUID** | References the price formula entity. | [optional] 
**default_tax_rate** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**gtin** | **str** |  | [optional] 
**height** | **str** |  | [optional] 
**image_link** | **str** |  | [optional] 
**images** | **object** |  | [optional] 
**is_taxable** | **bool** |  | [optional] 
**length** | **str** |  | [optional] 
**link** | **str** |  | [optional] 
**max_stock** | **int** | Target stock level used by reorder proposals. | [optional] 
**min_stock** | **int** | Reorder point — when stock falls below this, a reorder is suggested. | [optional] 
**mpn** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**package_height** | **str** |  | [optional] 
**package_length** | **str** |  | [optional] 
**package_weight_unit** | **str** |  | [optional] 
**package_weight_value** | **str** |  | [optional] 
**package_width** | **str** |  | [optional] 
**product_code** | **str** |  | [optional] 
**product_type** | **str** |  | [optional] 
**purchase_price** | **str** |  | [optional] 
**reorder_quantity** | **int** | Suggested purchase quantity when a reorder proposal is created. | [optional] 
**sale_price** | **str** |  | [optional] 
**shipping_price** | **str** |  | [optional] 
**shipping_requires_insurance** | **bool** |  | [optional] 
**sku** | **str** |  | [optional] 
**stock_quantity** | **int** |  | [optional] 
**tags** | **object** |  | [optional] 
**tax_price** | **str** |  | [optional] 
**track_batch** | **bool** | Whether this product requires batch (Chargennummer) tracking. | [optional] 
**track_serial** | **bool** | Whether this product requires serial-number tracking. | [optional] 
**unit** | **object** |  | [optional] 
**weight_unit** | **str** |  | [optional] 
**weight_value** | **str** |  | [optional] 
**width** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.product_update import ProductUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ProductUpdate from a JSON string
product_update_instance = ProductUpdate.from_json(json)
# print the JSON string representation of the object
print(ProductUpdate.to_json())

# convert the object into a dict
product_update_dict = product_update_instance.to_dict()
# create an instance of ProductUpdate from a dict
product_update_from_dict = ProductUpdate.from_dict(product_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


