# WarehouseCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_city** | **str** |  | [optional] 
**address_country** | [**CountryCode**](CountryCode.md) |  | [optional] 
**address_street** | **str** |  | [optional] 
**address_zip** | **str** |  | [optional] 
**bin_locations** | **object** | JSON array of bin locations, e.g. &#x60;[\&quot;A-01-01\&quot;, \&quot;A-01-02\&quot;]&#x60;. | [optional] 
**code** | **str** |  | 
**is_active** | **bool** |  | [optional] 
**is_default** | **bool** |  | [optional] 
**name** | **str** |  | 
**notes** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.warehouse_create import WarehouseCreate

# TODO update the JSON string below
json = "{}"
# create an instance of WarehouseCreate from a JSON string
warehouse_create_instance = WarehouseCreate.from_json(json)
# print the JSON string representation of the object
print(WarehouseCreate.to_json())

# convert the object into a dict
warehouse_create_dict = warehouse_create_instance.to_dict()
# create an instance of WarehouseCreate from a dict
warehouse_create_from_dict = WarehouseCreate.from_dict(warehouse_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


