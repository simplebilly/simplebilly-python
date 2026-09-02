# ProviderInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** |  | 
**name** | **str** |  | 
**requires_api_key** | **bool** |  | 
**services** | **List[str]** |  | 
**supports_label_creation** | **bool** |  | 
**supports_rate_estimation** | **bool** |  | 
**supports_tracking** | **bool** |  | 

## Example

```python
from simplebilly_api.models.provider_info import ProviderInfo

# TODO update the JSON string below
json = "{}"
# create an instance of ProviderInfo from a JSON string
provider_info_instance = ProviderInfo.from_json(json)
# print the JSON string representation of the object
print(ProviderInfo.to_json())

# convert the object into a dict
provider_info_dict = provider_info_instance.to_dict()
# create an instance of ProviderInfo from a dict
provider_info_from_dict = ProviderInfo.from_dict(provider_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


