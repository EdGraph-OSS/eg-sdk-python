# IdentityApiApiClientV1ApiClientCreatedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**secret_value** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_api_client_created_response import IdentityApiApiClientV1ApiClientCreatedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1ApiClientCreatedResponse from a JSON string
identity_api_api_client_v1_api_client_created_response_instance = IdentityApiApiClientV1ApiClientCreatedResponse.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1ApiClientCreatedResponse.to_json())

# convert the object into a dict
identity_api_api_client_v1_api_client_created_response_dict = identity_api_api_client_v1_api_client_created_response_instance.to_dict()
# create an instance of IdentityApiApiClientV1ApiClientCreatedResponse from a dict
identity_api_api_client_v1_api_client_created_response_from_dict = IdentityApiApiClientV1ApiClientCreatedResponse.from_dict(identity_api_api_client_v1_api_client_created_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


