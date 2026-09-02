# ComplianceTrainingCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assignable** | **bool** | Whether HR can assign this training as required for employees. | [optional] 
**code** | **str** | Stable code used by plugins and frontend players (e.g. \&quot;data_privacy\&quot;). | [optional] 
**description** | **str** |  | [optional] 
**pass_score** | **int** | Minimum score (0–100) required to pass. | [optional] 
**plugin_platform** | **str** | Marketplace plugin platform id when source &#x3D; Plugin. | [optional] 
**source** | [**TrainingSource**](TrainingSource.md) |  | [optional] 
**title** | **str** |  | [optional] 
**validity_months** | **int** | Certificate validity in months; null &#x3D; no expiry. | [optional] 

## Example

```python
from simplebilly_api.models.compliance_training_create import ComplianceTrainingCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ComplianceTrainingCreate from a JSON string
compliance_training_create_instance = ComplianceTrainingCreate.from_json(json)
# print the JSON string representation of the object
print(ComplianceTrainingCreate.to_json())

# convert the object into a dict
compliance_training_create_dict = compliance_training_create_instance.to_dict()
# create an instance of ComplianceTrainingCreate from a dict
compliance_training_create_from_dict = ComplianceTrainingCreate.from_dict(compliance_training_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


