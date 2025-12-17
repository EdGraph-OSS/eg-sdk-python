# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_name** | **str** | The user name for this user. | [optional] 
**email** | **str** | The email address for this user. | [optional] 
**first_name** | **str** | The first name for this user. | [optional] 
**last_name** | **str** | The last name for this user. | [optional] 
**preferences** | [**List[IdentityApiUserV1Preference]**](IdentityApiUserV1Preference.md) | List of preferences associated with this user | [optional] 
**tenants** | [**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse.md) | List of tenants associated with this user | [optional] 
**browser_debug_enabled** | **bool** | Flag to indicate if the debug mode for user is enabled | [optional] 
**extensions** | [**List[IdentityApiUserV1UserExtension]**](IdentityApiUserV1UserExtension.md) |  | [optional] 
**selected_tenant** | [**EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheTenantResponse.md) |  | [optional] 
**tenants_total_count** | **int** | The total count of active tenants associated with this user | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_response import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_response_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_response_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_response_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_response_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserCacheResponse.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_cache_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


