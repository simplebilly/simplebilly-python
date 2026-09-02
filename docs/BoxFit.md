# BoxFit


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**height_cm** | **float** |  | 
**item_count** | **int** |  | 
**length_cm** | **float** |  | 
**volume_cm3** | **float** |  | 
**width_cm** | **float** |  | 

## Example

```python
from simplebilly_api.models.box_fit import BoxFit

# TODO update the JSON string below
json = "{}"
# create an instance of BoxFit from a JSON string
box_fit_instance = BoxFit.from_json(json)
# print the JSON string representation of the object
print(BoxFit.to_json())

# convert the object into a dict
box_fit_dict = box_fit_instance.to_dict()
# create an instance of BoxFit from a dict
box_fit_from_dict = BoxFit.from_dict(box_fit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


