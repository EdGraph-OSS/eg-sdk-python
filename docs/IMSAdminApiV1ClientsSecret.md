# IMSAdminApiV1ClientsSecret


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**expiration** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_clients_secret import IMSAdminApiV1ClientsSecret

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ClientsSecret from a JSON string
ims_admin_api_v1_clients_secret_instance = IMSAdminApiV1ClientsSecret.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ClientsSecret.to_json())

# convert the object into a dict
ims_admin_api_v1_clients_secret_dict = ims_admin_api_v1_clients_secret_instance.to_dict()
# create an instance of IMSAdminApiV1ClientsSecret from a dict
ims_admin_api_v1_clients_secret_from_dict = IMSAdminApiV1ClientsSecret.from_dict(ims_admin_api_v1_clients_secret_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


