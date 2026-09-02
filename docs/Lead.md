# Lead


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**company** | **str** |  | [optional] 
**converted_at** | **datetime** |  | [optional] 
**created_at** | **datetime** |  | 
**email** | **str** |  | [optional] 
**first_contact_at** | **datetime** |  | 
**name** | **str** |  | 
**notes** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**score** | **int** |  | 
**source** | **str** |  | 
**status** | [**LeadStatus**](LeadStatus.md) |  | 
**tags** | **object** |  | 
**tenant_id** | **UUID** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.lead import Lead

# TODO update the JSON string below
json = "{}"
# create an instance of Lead from a JSON string
lead_instance = Lead.from_json(json)
# print the JSON string representation of the object
print(Lead.to_json())

# convert the object into a dict
lead_dict = lead_instance.to_dict()
# create an instance of Lead from a dict
lead_from_dict = Lead.from_dict(lead_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


