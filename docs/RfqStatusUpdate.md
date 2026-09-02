# RfqStatusUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | 

## Example

```python
from simplebilly_api.models.rfq_status_update import RfqStatusUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of RfqStatusUpdate from a JSON string
rfq_status_update_instance = RfqStatusUpdate.from_json(json)
# print the JSON string representation of the object
print(RfqStatusUpdate.to_json())

# convert the object into a dict
rfq_status_update_dict = rfq_status_update_instance.to_dict()
# create an instance of RfqStatusUpdate from a dict
rfq_status_update_from_dict = RfqStatusUpdate.from_dict(rfq_status_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


