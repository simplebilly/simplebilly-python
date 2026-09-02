# MarketplaceConnection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config** | **object** |  | 
**connection_id** | **str** |  | 
**connector_type** | [**ConnectorType**](ConnectorType.md) |  | 
**created_at** | **datetime** |  | 
**is_active** | **bool** |  | 
**label** | **str** |  | 
**last_sync_at** | **datetime** |  | [optional] 
**platform** | **str** |  | 
**platform_user_id** | **str** |  | [optional] 
**scopes** | **str** |  | [optional] 
**shop_domain** | **str** |  | [optional] 
**shop_name** | **str** |  | [optional] 
**sync_status** | **str** |  | [optional] 
**tenant_id** | **UUID** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from simplebilly_api.models.marketplace_connection import MarketplaceConnection

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceConnection from a JSON string
marketplace_connection_instance = MarketplaceConnection.from_json(json)
# print the JSON string representation of the object
print(MarketplaceConnection.to_json())

# convert the object into a dict
marketplace_connection_dict = marketplace_connection_instance.to_dict()
# create an instance of MarketplaceConnection from a dict
marketplace_connection_from_dict = MarketplaceConnection.from_dict(marketplace_connection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


