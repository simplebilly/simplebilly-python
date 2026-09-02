# OrderTagsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tags** | **List[str]** |  | 

## Example

```python
from simplebilly_api.models.order_tags_request import OrderTagsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OrderTagsRequest from a JSON string
order_tags_request_instance = OrderTagsRequest.from_json(json)
# print the JSON string representation of the object
print(OrderTagsRequest.to_json())

# convert the object into a dict
order_tags_request_dict = order_tags_request_instance.to_dict()
# create an instance of OrderTagsRequest from a dict
order_tags_request_from_dict = OrderTagsRequest.from_dict(order_tags_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


