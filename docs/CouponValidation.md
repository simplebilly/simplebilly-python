# CouponValidation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**discount_type** | **str** |  | 
**discount_value** | **str** |  | 
**discounted_amount** | **str** |  | 
**max_discount_amount** | **str** |  | [optional] 
**reason** | **str** |  | [optional] 
**valid** | **bool** |  | 

## Example

```python
from simplebilly_api.models.coupon_validation import CouponValidation

# TODO update the JSON string below
json = "{}"
# create an instance of CouponValidation from a JSON string
coupon_validation_instance = CouponValidation.from_json(json)
# print the JSON string representation of the object
print(CouponValidation.to_json())

# convert the object into a dict
coupon_validation_dict = coupon_validation_instance.to_dict()
# create an instance of CouponValidation from a dict
coupon_validation_from_dict = CouponValidation.from_dict(coupon_validation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


