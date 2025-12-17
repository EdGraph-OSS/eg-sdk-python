# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_name** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**secret** | **str** |  | [optional] 
**allowed_scopes** | **List[str]** |  | [optional] 
**claims** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterClaimDto]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterClaimDto.md) |  | [optional] 
**application_id** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**logo_uri** | **str** |  | [optional] 
**client_uri** | **str** |  | [optional] 
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
**require_pkce** | **bool** |  | [optional] 
**allowed_cors_origins** | **List[str]** |  | [optional] 
**allowed_grant_types** | **List[str]** |  | [optional] 
**identity_provider_restrictions** | **List[str]** |  | [optional] 
**redirect_uris** | **List[str]** |  | [optional] 
**post_logout_redirect_uris** | **List[str]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsOneRosterCreateClientRequestDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_one_roster_create_client_request_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


