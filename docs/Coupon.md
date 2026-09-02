# Coupon


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**description** | **str** |  | [optional] 
**discount_type** | [**DiscountType**](DiscountType.md) |  | 
**discount_value** | **str** |  | 
**expires_at** | **datetime** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**is_combineable** | **bool** |  | [optional] 
**max_discount_amount** | **str** |  | [optional] 
**max_uses** | **int** |  | [optional] 
**max_uses_per_customer** | **int** |  | [optional] 
**min_order_amount** | **str** |  | [optional] 
**product_ids** | **object** |  | [optional] 
**starts_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.coupon import Coupon

# TODO update the JSON string below
json = "{}"
# create an instance of Coupon from a JSON string
coupon_instance = Coupon.from_json(json)
# print the JSON string representation of the object
print(Coupon.to_json())

# convert the object into a dict
coupon_dict = coupon_instance.to_dict()
# create an instance of Coupon from a dict
coupon_from_dict = Coupon.from_dict(coupon_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


