# Verfahrensdokumentation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**entries** | [**List[ComplianceEntry]**](ComplianceEntry.md) |  | 
**generated_at** | **str** |  | 
**title** | **str** |  | 
**version** | **str** |  | 

## Example

```python
from simplebilly_api.models.verfahrensdokumentation import Verfahrensdokumentation

# TODO update the JSON string below
json = "{}"
# create an instance of Verfahrensdokumentation from a JSON string
verfahrensdokumentation_instance = Verfahrensdokumentation.from_json(json)
# print the JSON string representation of the object
print(Verfahrensdokumentation.to_json())

# convert the object into a dict
verfahrensdokumentation_dict = verfahrensdokumentation_instance.to_dict()
# create an instance of Verfahrensdokumentation from a dict
verfahrensdokumentation_from_dict = Verfahrensdokumentation.from_dict(verfahrensdokumentation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


