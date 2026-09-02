# InstituteDeadlines


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**abschlusspruefung_months** | **int** | HGB § 340k/§ 341k: Abschlussprüfung (5 Monate). | [optional] 
**jahresabschluss_bafin_months** | **int** | KWG § 26: Jahresabschluss an die BaFin (3 Monate, nur KWG-Institute). | [optional] 
**offenlegung_months** | **int** | HGB § 325 Abs. 4: Offenlegung (4 kapitalmarktorientiert / 12 sonst). | 

## Example

```python
from simplebilly_api.models.institute_deadlines import InstituteDeadlines

# TODO update the JSON string below
json = "{}"
# create an instance of InstituteDeadlines from a JSON string
institute_deadlines_instance = InstituteDeadlines.from_json(json)
# print the JSON string representation of the object
print(InstituteDeadlines.to_json())

# convert the object into a dict
institute_deadlines_dict = institute_deadlines_instance.to_dict()
# create an instance of InstituteDeadlines from a dict
institute_deadlines_from_dict = InstituteDeadlines.from_dict(institute_deadlines_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


