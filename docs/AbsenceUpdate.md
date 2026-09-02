# AbsenceUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**absence_type** | [**AbsenceType**](AbsenceType.md) | One of \&quot;vacation\&quot;, \&quot;sick\&quot;, \&quot;sabbatical\&quot;, \&quot;parental\&quot;, \&quot;other\&quot;. | [optional] 
**approved_at** | **datetime** |  | [optional] 
**approved_by** | **UUID** | References the user entity. | [optional] 
**employee_id** | **UUID** | References the employee entity. | [optional] 
**end_date** | **date** |  | [optional] 
**notes** | **str** |  | [optional] 
**start_date** | **date** |  | [optional] 
**status** | [**AbsenceStatus**](AbsenceStatus.md) | One of \&quot;pending\&quot;, \&quot;approved\&quot;, \&quot;rejected\&quot;, \&quot;cancelled\&quot;. | [optional] 

## Example

```python
from simplebilly_api.models.absence_update import AbsenceUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AbsenceUpdate from a JSON string
absence_update_instance = AbsenceUpdate.from_json(json)
# print the JSON string representation of the object
print(AbsenceUpdate.to_json())

# convert the object into a dict
absence_update_dict = absence_update_instance.to_dict()
# create an instance of AbsenceUpdate from a dict
absence_update_from_dict = AbsenceUpdate.from_dict(absence_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


