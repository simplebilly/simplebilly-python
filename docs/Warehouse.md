# Warehouse


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
from simplebilly_api.models.warehouse import Warehouse

# TODO update the JSON string below
json = "{}"
# create an instance of Warehouse from a JSON string
warehouse_instance = Warehouse.from_json(json)
# print the JSON string representation of the object
print(Warehouse.to_json())

# convert the object into a dict
warehouse_dict = warehouse_instance.to_dict()
# create an instance of Warehouse from a dict
warehouse_from_dict = Warehouse.from_dict(warehouse_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


