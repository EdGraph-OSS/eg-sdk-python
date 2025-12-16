# IdentityApiApiClientV1RegenerateApiClientSecretRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**secret_expiration_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_regenerate_api_client_secret_request import IdentityApiApiClientV1RegenerateApiClientSecretRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1RegenerateApiClientSecretRequest from a JSON string
identity_api_api_client_v1_regenerate_api_client_secret_request_instance = IdentityApiApiClientV1RegenerateApiClientSecretRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1RegenerateApiClientSecretRequest.to_json())

# convert the object into a dict
identity_api_api_client_v1_regenerate_api_client_secret_request_dict = identity_api_api_client_v1_regenerate_api_client_secret_request_instance.to_dict()
# create an instance of IdentityApiApiClientV1RegenerateApiClientSecretRequest from a dict
identity_api_api_client_v1_regenerate_api_client_secret_request_from_dict = IdentityApiApiClientV1RegenerateApiClientSecretRequest.from_dict(identity_api_api_client_v1_regenerate_api_client_secret_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


