# IMSAdminApiV1ClientsClientSecretAddedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**secret_value** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**expiration** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_secret_added_response import IMSAdminApiV1ClientsClientSecretAddedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ClientsClientSecretAddedResponse from a JSON string
ims_admin_api_v1_clients_client_secret_added_response_instance = IMSAdminApiV1ClientsClientSecretAddedResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ClientsClientSecretAddedResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_clients_client_secret_added_response_dict = ims_admin_api_v1_clients_client_secret_added_response_instance.to_dict()
# create an instance of IMSAdminApiV1ClientsClientSecretAddedResponse from a dict
ims_admin_api_v1_clients_client_secret_added_response_from_dict = IMSAdminApiV1ClientsClientSecretAddedResponse.from_dict(ims_admin_api_v1_clients_client_secret_added_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


