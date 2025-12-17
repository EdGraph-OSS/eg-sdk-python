# EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**api_client_id** | **int** |  | [optional] 
**new_secret** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_regenerate_api_client_secret_response import EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse from a JSON string
edfi_admin_api_edfi_admin_v1_regenerate_api_client_secret_response_instance = EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_regenerate_api_client_secret_response_dict = edfi_admin_api_edfi_admin_v1_regenerate_api_client_secret_response_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse from a dict
edfi_admin_api_edfi_admin_v1_regenerate_api_client_secret_response_from_dict = EdfiAdminApiEdfiAdminV1RegenerateApiClientSecretResponse.from_dict(edfi_admin_api_edfi_admin_v1_regenerate_api_client_secret_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


