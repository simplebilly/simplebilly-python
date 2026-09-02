# ApiResponseGdprExportData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activity_log** | [**List[GdprActivity]**](GdprActivity.md) |  | 
**api_keys** | [**List[GdprApiKey]**](GdprApiKey.md) | Key identifiers and names only — never a usable credential. | 
**billing** | [**List[GdprBillingInfo]**](GdprBillingInfo.md) |  | 
**exported_at** | **datetime** |  | 
**generated_by_ai** | **bool** | Honesty field: this document is a plain data dump, never AI-generated. | 
**notifications** | [**List[GdprNotification]**](GdprNotification.md) |  | 
**refresh_tokens** | [**List[GdprRefreshToken]**](GdprRefreshToken.md) | Session records: metadata only, never the token hash. | 
**tenants** | [**List[GdprTenant]**](GdprTenant.md) |  | 
**usage_events** | [**List[GdprUsageEvent]**](GdprUsageEvent.md) |  | 
**user** | [**GdprUser**](GdprUser.md) |  | 

## Example

```python
from simplebilly_api.models.api_response_gdpr_export_data import ApiResponseGdprExportData

# TODO update the JSON string below
json = "{}"
# create an instance of ApiResponseGdprExportData from a JSON string
api_response_gdpr_export_data_instance = ApiResponseGdprExportData.from_json(json)
# print the JSON string representation of the object
print(ApiResponseGdprExportData.to_json())

# convert the object into a dict
api_response_gdpr_export_data_dict = api_response_gdpr_export_data_instance.to_dict()
# create an instance of ApiResponseGdprExportData from a dict
api_response_gdpr_export_data_from_dict = ApiResponseGdprExportData.from_dict(api_response_gdpr_export_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


