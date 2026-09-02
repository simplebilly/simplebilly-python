# Address


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**city** | **str** |  | 
**company** | **str** |  | [optional] 
**country** | **str** | ISO 3166-1 alpha-2 country code (e.g. \&quot;DE\&quot;, \&quot;PL\&quot;, \&quot;FR\&quot;). | 
**email** | **str** |  | [optional] 
**name** | **str** |  | 
**phone** | **str** |  | [optional] 
**street** | **str** |  | 
**street_number** | **str** |  | 
**zip** | **str** |  | 

## Example

```python
from simplebilly_api.models.address import Address

# TODO update the JSON string below
json = "{}"
# create an instance of Address from a JSON string
address_instance = Address.from_json(json)
# print the JSON string representation of the object
print(Address.to_json())

# convert the object into a dict
address_dict = address_instance.to_dict()
# create an instance of Address from a dict
address_from_dict = Address.from_dict(address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


