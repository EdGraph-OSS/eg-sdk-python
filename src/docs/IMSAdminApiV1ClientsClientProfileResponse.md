# IMSAdminApiV1ClientsClientProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**client_uri** | **str** |  | [optional] 
**logo_uri** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**access_token_type** | [**IMSAdminApiV1ClientsAccessTokenType**](IMSAdminApiV1ClientsAccessTokenType.md) |  | [optional] 
**token_usage** | [**IMSAdminApiV1ClientsTokenUsage**](IMSAdminApiV1ClientsTokenUsage.md) |  | [optional] 
**refresh_token_expiration** | [**IMSAdminApiV1ClientsTokenExpiration**](IMSAdminApiV1ClientsTokenExpiration.md) |  | [optional] 
**enable_local_login** | **bool** |  | [optional] 
**allow_offline_access** | **bool** |  | [optional] 
**allow_access_tokens_via_browser** | **bool** |  | [optional] 
**update_access_token_claims_on_refresh** | **bool** |  | [optional] 
**always_include_user_claims_in_id_token** | **bool** |  | [optional] 
**identity_token_lifetime** | **int** |  | [optional] 
**access_token_lifetime** | **int** |  | [optional] 
**authorization_code_lifetime** | **int** |  | [optional] 
**absolute_refresh_token_lifetime** | **int** |  | [optional] 
**sliding_refresh_token_lifetime** | **int** |  | [optional] 
**require_client_secret** | **bool** |  | [optional] 
**require_consent** | **bool** |  | [optional] 
**allowed_scopes** | **List[str]** |  | [optional] [readonly] 
**allowed_cors_origins** | **List[str]** |  | [optional] [readonly] 
**allowed_grant_types** | **List[str]** |  | [optional] [readonly] 
**identity_provider_restrictions** | **List[str]** |  | [optional] [readonly] 
**redirect_uris** | **List[str]** |  | [optional] [readonly] 
**post_logout_redirect_uris** | **List[str]** |  | [optional] [readonly] 
**client_secrets** | [**List[IMSAdminApiV1ClientsSecret]**](IMSAdminApiV1ClientsSecret.md) |  | [optional] [readonly] 
**claims** | [**List[IMSAdminApiV1ClientsClaim]**](IMSAdminApiV1ClientsClaim.md) |  | [optional] [readonly] 
**require_pkce** | **bool** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**instance_id** | **str** |  | [optional] 
**selected_scope** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ims_admin_api_v1_clients_client_profile_response import IMSAdminApiV1ClientsClientProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of IMSAdminApiV1ClientsClientProfileResponse from a JSON string
ims_admin_api_v1_clients_client_profile_response_instance = IMSAdminApiV1ClientsClientProfileResponse.from_json(json)
# print the JSON string representation of the object
print(IMSAdminApiV1ClientsClientProfileResponse.to_json())

# convert the object into a dict
ims_admin_api_v1_clients_client_profile_response_dict = ims_admin_api_v1_clients_client_profile_response_instance.to_dict()
# create an instance of IMSAdminApiV1ClientsClientProfileResponse from a dict
ims_admin_api_v1_clients_client_profile_response_from_dict = IMSAdminApiV1ClientsClientProfileResponse.from_dict(ims_admin_api_v1_clients_client_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


