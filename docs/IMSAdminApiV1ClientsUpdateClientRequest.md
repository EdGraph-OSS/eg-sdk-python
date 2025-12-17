# IMSAdminApiV1ClientsUpdateClientRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**allowed_scopes** | **List[str]** |  | [optional] [readonly] 
**claims** | [**List[IMSAdminApiV1ClientsClaim]**](IMSAdminApiV1ClientsClaim.md) |  | [optional] [readonly] 
**instance_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_clients_update_client_request import IMSAdminApiV1ClientsUpdateClientRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ClientsUpdateClientRequest from a JSON string
ims_admin_api_v1_clients_update_client_request_instance = IMSAdminApiV1ClientsUpdateClientRequest.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ClientsUpdateClientRequest.to_json())

# convert the object into a dict
ims_admin_api_v1_clients_update_client_request_dict = ims_admin_api_v1_clients_update_client_request_instance.to_dict()
# create an instance of IMSAdminApiV1ClientsUpdateClientRequest from a dict
ims_admin_api_v1_clients_update_client_request_from_dict = IMSAdminApiV1ClientsUpdateClientRequest.from_dict(ims_admin_api_v1_clients_update_client_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


