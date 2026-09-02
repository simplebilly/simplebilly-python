# PayGapInfoResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**employee_id** | **UUID** |  | 
**first_name** | **str** |  | 
**gender** | **str** |  | [optional] 
**group_median_hourly** | **float** |  | [optional] 
**group_median_monthly** | **float** |  | [optional] 
**group_size** | **int** |  | 
**job_title** | **str** |  | 
**last_name** | **str** |  | 
**overall_median_hourly** | **float** |  | [optional] 
**own_hourly_gross** | **float** |  | [optional] 
**own_monthly_gross** | **float** |  | [optional] 

## Example

```python
from simplebilly_api.models.pay_gap_info_response import PayGapInfoResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PayGapInfoResponse from a JSON string
pay_gap_info_response_instance = PayGapInfoResponse.from_json(json)
# print the JSON string representation of the object
print(PayGapInfoResponse.to_json())

# convert the object into a dict
pay_gap_info_response_dict = pay_gap_info_response_instance.to_dict()
# create an instance of PayGapInfoResponse from a dict
pay_gap_info_response_from_dict = PayGapInfoResponse.from_dict(pay_gap_info_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


