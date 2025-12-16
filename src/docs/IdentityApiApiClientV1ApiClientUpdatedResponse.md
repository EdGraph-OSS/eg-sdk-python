# IdentityApiApiClientV1ApiClientUpdatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_updated_response import IdentityApiApiClientV1ApiClientUpdatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1ApiClientUpdatedResponse from a JSON string
identity_api_api_client_v1_api_client_updated_response_instance = IdentityApiApiClientV1ApiClientUpdatedResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1ApiClientUpdatedResponse.to_json())

# convert the object into a dict
identity_api_api_client_v1_api_client_updated_response_dict = identity_api_api_client_v1_api_client_updated_response_instance.to_dict()
# create an instance of IdentityApiApiClientV1ApiClientUpdatedResponse from a dict
identity_api_api_client_v1_api_client_updated_response_from_dict = IdentityApiApiClientV1ApiClientUpdatedResponse.from_dict(identity_api_api_client_v1_api_client_updated_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


