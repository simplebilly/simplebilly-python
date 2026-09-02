# ApplicationFilter


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**posting_id** | **UUID** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.application_filter import ApplicationFilter

# TODO update the JSON string below
json = "{}"
# create an instance of ApplicationFilter from a JSON string
application_filter_instance = ApplicationFilter.from_json(json)
# print the JSON string representation of the object
print(ApplicationFilter.to_json())

# convert the object into a dict
application_filter_dict = application_filter_instance.to_dict()
# create an instance of ApplicationFilter from a dict
application_filter_from_dict = ApplicationFilter.from_dict(application_filter_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


