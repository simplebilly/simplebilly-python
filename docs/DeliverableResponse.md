# DeliverableResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available_stock** | **int** |  | 
**deliverable_quantity** | **int** |  | 
**max_sellable** | **int** |  | [optional] 
**product_id** | **UUID** |  | 
**reserved_stock** | **int** |  | 
**warehouse_id** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.deliverable_response import DeliverableResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DeliverableResponse from a JSON string
deliverable_response_instance = DeliverableResponse.from_json(json)
# print the JSON string representation of the object
print(DeliverableResponse.to_json())

# convert the object into a dict
deliverable_response_dict = deliverable_response_instance.to_dict()
# create an instance of DeliverableResponse from a dict
deliverable_response_from_dict = DeliverableResponse.from_dict(deliverable_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


