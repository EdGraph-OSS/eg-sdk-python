# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserListResponseWithApplicationLicense


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**user_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**tenant_count** | **int** |  | [optional] 
**tenants** | [**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenant]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserTenant.md) |  | [optional] 
**licenses** | [**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicense]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicense.md) |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**logins** | [**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLogin]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLogin.md) |  | [optional] 
**source** | **str** |  | [optional] 
**last_login_date_time** | **str** |  | [optional] 
**mfa_completed** | **bool** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_list_response_with_application_license import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserListResponseWithApplicationLicense

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserListResponseWithApplicationLicense from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_list_response_with_application_license_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserListResponseWithApplicationLicense.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserListResponseWithApplicationLicense.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_list_response_with_application_license_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_list_response_with_application_license_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserListResponseWithApplicationLicense from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_list_response_with_application_license_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserListResponseWithApplicationLicense.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_list_response_with_application_license_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


