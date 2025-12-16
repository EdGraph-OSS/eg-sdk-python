# IdentityApiApiClientV1CreateApiClientRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**client_name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**api_claims** | [**List[IdentityApiApiClientV1ApiClaim]**](IdentityApiApiClientV1ApiClaim.md) |  | [optional] [readonly] 
**secret_expiration_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.identity_api_api_client_v1_create_api_client_request import IdentityApiApiClientV1CreateApiClientRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityApiApiClientV1CreateApiClientRequest from a JSON string
identity_api_api_client_v1_create_api_client_request_instance = IdentityApiApiClientV1CreateApiClientRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityApiApiClientV1CreateApiClientRequest.to_json())

# convert the object into a dict
identity_api_api_client_v1_create_api_client_request_dict = identity_api_api_client_v1_create_api_client_request_instance.to_dict()
# create an instance of IdentityApiApiClientV1CreateApiClientRequest from a dict
identity_api_api_client_v1_create_api_client_request_from_dict = IdentityApiApiClientV1CreateApiClientRequest.from_dict(identity_api_api_client_v1_create_api_client_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


