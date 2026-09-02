# HebesatzLookup


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bundesland** | **str** |  | 
**country_code** | **str** |  | 
**gemeinde_name** | **str** |  | 
**gemeindeschluessel** | **str** |  | 
**hebesatz_gewerbesteuer** | **float** |  | 
**hebesatz_grundsteuer_b** | **float** |  | [optional] 
**jahr** | **int** |  | 
**landkreis** | **str** |  | [optional] 
**valid_from** | **str** |  | 
**valid_to** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.hebesatz_lookup import HebesatzLookup

# TODO update the JSON string below
json = "{}"
# create an instance of HebesatzLookup from a JSON string
hebesatz_lookup_instance = HebesatzLookup.from_json(json)
# print the JSON string representation of the object
print(HebesatzLookup.to_json())

# convert the object into a dict
hebesatz_lookup_dict = hebesatz_lookup_instance.to_dict()
# create an instance of HebesatzLookup from a dict
hebesatz_lookup_from_dict = HebesatzLookup.from_dict(hebesatz_lookup_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


