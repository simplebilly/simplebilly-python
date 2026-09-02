# OssReport


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dependencies** | [**List[OssDependency]**](OssDependency.md) |  | 
**total_count** | **int** |  | 

## Example

```python
from simplebilly_api.models.oss_report import OssReport

# TODO update the JSON string below
json = "{}"
# create an instance of OssReport from a JSON string
oss_report_instance = OssReport.from_json(json)
# print the JSON string representation of the object
print(OssReport.to_json())

# convert the object into a dict
oss_report_dict = oss_report_instance.to_dict()
# create an instance of OssReport from a dict
oss_report_from_dict = OssReport.from_dict(oss_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


