# ShippingRuleUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**carrier** | **str** | Provider that auto-filled this rule (e.g. \&quot;ups\&quot;), if any. | [optional] 
**country** | [**CountryCode**](CountryCode.md) | None &#x3D; applies to all countries. | [optional] 
**delivery_time** | **str** | Delivery time text, e.g. \&quot;1-3\&quot;. | [optional] 
**is_active** | **bool** |  | [optional] 
**max_weight_kg** | **float** |  | [optional] 
**min_weight_kg** | **float** |  | [optional] 
**name** | **str** | Delivery-method label, e.g. \&quot;Standardversand\&quot;. | [optional] 
**notes** | **str** |  | [optional] 
**price** | **str** | Shipping cost in the shop&#39;s currency. | [optional] 
**priority** | **int** | Lower wins when multiple rules match. | [optional] 

## Example

```python
from simplebilly_api.models.shipping_rule_update import ShippingRuleUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ShippingRuleUpdate from a JSON string
shipping_rule_update_instance = ShippingRuleUpdate.from_json(json)
# print the JSON string representation of the object
print(ShippingRuleUpdate.to_json())

# convert the object into a dict
shipping_rule_update_dict = shipping_rule_update_instance.to_dict()
# create an instance of ShippingRuleUpdate from a dict
shipping_rule_update_from_dict = ShippingRuleUpdate.from_dict(shipping_rule_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


