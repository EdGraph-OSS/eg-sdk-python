# IMSAdminApiV1ClientsRegenerateClientSecretRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**secret_expiration_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_clients_regenerate_client_secret_request import IMSAdminApiV1ClientsRegenerateClientSecretRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ClientsRegenerateClientSecretRequest from a JSON string
ims_admin_api_v1_clients_regenerate_client_secret_request_instance = IMSAdminApiV1ClientsRegenerateClientSecretRequest.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ClientsRegenerateClientSecretRequest.to_json())

# convert the object into a dict
ims_admin_api_v1_clients_regenerate_client_secret_request_dict = ims_admin_api_v1_clients_regenerate_client_secret_request_instance.to_dict()
# create an instance of IMSAdminApiV1ClientsRegenerateClientSecretRequest from a dict
ims_admin_api_v1_clients_regenerate_client_secret_request_from_dict = IMSAdminApiV1ClientsRegenerateClientSecretRequest.from_dict(ims_admin_api_v1_clients_regenerate_client_secret_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


