# SupplierConditionCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **str** | Currency for the minimum order value. | 
**delivery_terms** | **str** | Incoterms, e.g. \&quot;EXW\&quot;, \&quot;DAP\&quot;. | [optional] 
**early_payment_discount_percent** | **str** | Early-payment discount percentage (Skonto), e.g. 2.0. | [optional] 
**is_default** | **bool** | Is this the default condition for the supplier? | [optional] 
**minimum_order_value** | **str** | Minimum order value required for this supplier. | [optional] 
**notes** | **str** |  | [optional] 
**payment_due_days** | **int** | Number of days within which payment is due. | [optional] 
**payment_terms** | **str** | Payment terms, e.g. \&quot;14 Tage, 2% Skonto\&quot;. | [optional] 
**supplier_contact_id** | **str** | The supplier this condition applies to (&#x60;contact_id&#x60;). References the supplier entity. | 
**supplier_name** | **str** | The name of the supplier, denormalized for easy listing. | [optional] 
**volume_discount_tiers** | **object** | Tiered discounts: JSON array of &#x60;{min_quantity, discount_percent}&#x60;. | [optional] 

## Example

```python
from simplebilly_api.models.supplier_condition_create import SupplierConditionCreate

# TODO update the JSON string below
json = "{}"
# create an instance of SupplierConditionCreate from a JSON string
supplier_condition_create_instance = SupplierConditionCreate.from_json(json)
# print the JSON string representation of the object
print(SupplierConditionCreate.to_json())

# convert the object into a dict
supplier_condition_create_dict = supplier_condition_create_instance.to_dict()
# create an instance of SupplierConditionCreate from a dict
supplier_condition_create_from_dict = SupplierConditionCreate.from_dict(supplier_condition_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


