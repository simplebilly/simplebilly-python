# PackingVideoResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | 
**recording_url** | **str** |  | [optional] 
**success** | **bool** |  | 

## Example

```python
from simplebilly_api.models.packing_video_response import PackingVideoResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PackingVideoResponse from a JSON string
packing_video_response_instance = PackingVideoResponse.from_json(json)
# print the JSON string representation of the object
print(PackingVideoResponse.to_json())

# convert the object into a dict
packing_video_response_dict = packing_video_response_instance.to_dict()
# create an instance of PackingVideoResponse from a dict
packing_video_response_from_dict = PackingVideoResponse.from_dict(packing_video_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


