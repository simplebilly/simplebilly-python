# WarehouseUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_city** | **str** |  | [optional] 
**address_country** | [**CountryCode**](CountryCode.md) |  | [optional] 
**address_street** | **str** |  | [optional] 
**address_zip** | **str** |  | [optional] 
**bin_locations** | **object** | JSON array of bin locations, e.g. &#x60;[\&quot;A-01-01\&quot;, \&quot;A-01-02\&quot;]&#x60;. | [optional] 
**code** | **str** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**is_default** | **bool** |  | [optional] 
**name** | **str** |  | [optional] 
**notes** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.warehouse_update import WarehouseUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of WarehouseUpdate from a JSON string
warehouse_update_instance = WarehouseUpdate.from_json(json)
# print the JSON string representation of the object
print(WarehouseUpdate.to_json())

# convert the object into a dict
warehouse_update_dict = warehouse_update_instance.to_dict()
# create an instance of WarehouseUpdate from a dict
warehouse_update_from_dict = WarehouseUpdate.from_dict(warehouse_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


