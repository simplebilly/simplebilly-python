# EmissionEntry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**activity_value** | **str** | Activity amount in &#x60;unit&#x60; (kWh, l, km, t, tkm, EUR). | 
**category_id** | **str** | GHG-Protocol category key, e.g. \&quot;purchased_goods\&quot;, \&quot;business_travel\&quot;. | 
**description** | **str** |  | 
**ef_source** | **str** | Emission-factor source, e.g. \&quot;UBA-2024\&quot;, \&quot;DEFRA-2024\&quot;. | 
**ef_version** | **str** |  | 
**method** | [**EmissionMethod**](EmissionMethod.md) | \&quot;activity\&quot; | \&quot;spend\&quot; | \&quot;supplier\&quot;. | 
**scope** | [**GhgScope**](GhgScope.md) | GHG scope: \&quot;1\&quot; | \&quot;2\&quot; | \&quot;3\&quot;. | 
**tco2e** | **str** | Computed server-side: activity * factor / 1000, rounded to 4 dp. | 
**unit** | **str** | Unit of the activity value. | 
**updated_at** | **datetime** |  | [optional] 
**year** | **int** | Reporting year. | 

## Example

```python
from simplebilly_api.models.emission_entry import EmissionEntry

# TODO update the JSON string below
json = "{}"
# create an instance of EmissionEntry from a JSON string
emission_entry_instance = EmissionEntry.from_json(json)
# print the JSON string representation of the object
print(EmissionEntry.to_json())

# convert the object into a dict
emission_entry_dict = emission_entry_instance.to_dict()
# create an instance of EmissionEntry from a dict
emission_entry_from_dict = EmissionEntry.from_dict(emission_entry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


