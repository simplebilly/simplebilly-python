# LeadUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**company** | **str** |  | [optional] 
**converted_at** | **datetime** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**email** | **str** |  | [optional] 
**first_contact_at** | **datetime** |  | [optional] 
**name** | **str** |  | [optional] 
**notes** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**score** | **int** |  | [optional] 
**source** | **str** |  | [optional] 
**status** | [**LeadStatus**](LeadStatus.md) |  | [optional] 
**tags** | **object** |  | [optional] 
**tenant_id** | **UUID** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.lead_update import LeadUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of LeadUpdate from a JSON string
lead_update_instance = LeadUpdate.from_json(json)
# print the JSON string representation of the object
print(LeadUpdate.to_json())

# convert the object into a dict
lead_update_dict = lead_update_instance.to_dict()
# create an instance of LeadUpdate from a dict
lead_update_from_dict = LeadUpdate.from_dict(lead_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


