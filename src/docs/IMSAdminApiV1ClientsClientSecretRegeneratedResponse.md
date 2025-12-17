# IMSAdminApiV1ClientsClientSecretRegeneratedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**secret_value** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_secret_regenerated_response import IMSAdminApiV1ClientsClientSecretRegeneratedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ClientsClientSecretRegeneratedResponse from a JSON string
ims_admin_api_v1_clients_client_secret_regenerated_response_instance = IMSAdminApiV1ClientsClientSecretRegeneratedResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ClientsClientSecretRegeneratedResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_clients_client_secret_regenerated_response_dict = ims_admin_api_v1_clients_client_secret_regenerated_response_instance.to_dict()
# create an instance of IMSAdminApiV1ClientsClientSecretRegeneratedResponse from a dict
ims_admin_api_v1_clients_client_secret_regenerated_response_from_dict = IMSAdminApiV1ClientsClientSecretRegeneratedResponse.from_dict(ims_admin_api_v1_clients_client_secret_regenerated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


