# Absence


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**absence_type** | [**AbsenceType**](AbsenceType.md) | One of \&quot;vacation\&quot;, \&quot;sick\&quot;, \&quot;sabbatical\&quot;, \&quot;parental\&quot;, \&quot;other\&quot;. | [optional] 
**approved_at** | **datetime** |  | [optional] 
**approved_by** | **UUID** | References the user entity. | [optional] 
**created_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**employee_id** | **UUID** | References the employee entity. | [optional] 
**end_date** | **date** |  | [optional] 
**id** | **UUID** |  | [optional] 
**notes** | **str** |  | [optional] 
**start_date** | **date** |  | [optional] 
**status** | [**AbsenceStatus**](AbsenceStatus.md) | One of \&quot;pending\&quot;, \&quot;approved\&quot;, \&quot;rejected\&quot;, \&quot;cancelled\&quot;. | [optional] 
**tenant_id** | **UUID** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.absence import Absence

# TODO update the JSON string below
json = "{}"
# create an instance of Absence from a JSON string
absence_instance = Absence.from_json(json)
# print the JSON string representation of the object
print(Absence.to_json())

# convert the object into a dict
absence_dict = absence_instance.to_dict()
# create an instance of Absence from a dict
absence_from_dict = Absence.from_dict(absence_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


