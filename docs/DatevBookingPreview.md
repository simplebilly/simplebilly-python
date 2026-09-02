# DatevBookingPreview


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_number** | **str** |  | 
**debit_credit** | **str** |  | 
**document_date** | **str** |  | 
**document_text** | **str** |  | 
**net_amount** | **str** |  | 
**opposite_account** | **str** |  | 
**tax_amount** | **str** |  | [optional] 
**tax_rate** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.datev_booking_preview import DatevBookingPreview

# TODO update the JSON string below
json = "{}"
# create an instance of DatevBookingPreview from a JSON string
datev_booking_preview_instance = DatevBookingPreview.from_json(json)
# print the JSON string representation of the object
print(DatevBookingPreview.to_json())

# convert the object into a dict
datev_booking_preview_dict = datev_booking_preview_instance.to_dict()
# create an instance of DatevBookingPreview from a dict
datev_booking_preview_from_dict = DatevBookingPreview.from_dict(datev_booking_preview_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


