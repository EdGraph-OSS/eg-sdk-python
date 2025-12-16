# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicense


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription_tenant_id** | **str** | The Tenant Id the subscription belongs to | [optional] 
**is_tenant_subscribed** | **bool** | The Tenant has a subscription license for this application | [optional] 
**tenant_subscription_id** | **str** | The Tenant subscription Id | [optional] 
**tenant_subscription_start_date_time** | **str** | The Tenant subscription start date | [optional] 
**tenant_subscription_end_date_time** | **str** | The Tenant subscription end date | [optional] 
**tenant_subscription_actual_end_date_time** | **str** | The Tenant subscription end date | [optional] 
**tenant_subscription_deleted_at** | **str** | The Tenant subscription deleted date | [optional] 
**tenant_subscription_grace_period** | **int** | The Tenant subscription grace period value | [optional] 
**number_of_licenses** | **int** | The Tenant&#39;s number of licenses | [optional] 
**assigned_licenses** | **int** | The Tenant&#39;s assigned of licenses | [optional] 
**is_user_licensed** | **bool** | The user is assigned license for this application | [optional] 
**application_tenant_id** | **str** | The Tenant this application belongs to | [optional] 
**application_id** | **str** | The application Id of the application for license | [optional] 
**application_name** | **str** | The application Name of the application for license | [optional] 
**application_role** | [**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationRole]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationRole.md) | Application role for this user. | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_license import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicense

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicense from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_license_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicense.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicense.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_license_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_license_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicense from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_license_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesUserLicense.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_user_license_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


