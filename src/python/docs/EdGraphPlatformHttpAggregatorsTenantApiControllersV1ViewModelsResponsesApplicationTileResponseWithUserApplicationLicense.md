# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTileResponseWithUserApplicationLicense


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application_tenant_id** | **str** | The Tenant this application belongs to | [optional] 
**application_id** | **str** |  | [optional] 
**application_name** | **str** |  | [optional] 
**application_description** | **str** |  | [optional] 
**documentation_url** | **str** |  | [optional] 
**application_uri** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**tooltip_text** | **str** |  | [optional] 
**tags** | **str** |  | [optional] 
**groups** | **str** |  | [optional] 
**light_icon_url** | **str** |  | [optional] 
**dark_icon_url** | **str** |  | [optional] 
**light_background_tile_url** | **str** |  | [optional] 
**dark_background_tile_url** | **str** |  | [optional] 
**light_overlay_tile_url** | **str** |  | [optional] 
**dark_overlay_tile_url** | **str** |  | [optional] 
**show_in_app_launcher** | **bool** |  | [optional] 
**show_in_quick_launcher** | **bool** |  | [optional] 
**open_in_new_window** | **bool** |  | [optional] 
**is_tenant_subscribed** | **bool** |  | [optional] 
**subscription_tenant_id** | **str** | The Tenant Id the subscription belongs to | [optional] 
**tenant_subscription_id** | **str** | The Tenant subscription Id | [optional] 
**tenant_subscription_start_date_time** | **str** | The Tenant subscription start date | [optional] 
**tenant_subscription_end_date_time** | **str** | The Tenant subscription end date | [optional] 
**tenant_subscription_actual_end_date_time** | **str** | The Tenant subscription end date | [optional] 
**tenant_subscription_deleted_at** | **str** | The Tenant subscription deleted date | [optional] 
**tenant_subscription_grace_period** | **int** | The Tenant subscription grace period value | [optional] 
**is_user_licensed** | **bool** |  | [optional] 
**urls** | [**List[EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationUrl]**](EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationUrl.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_application_tile_response_with_user_application_license import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTileResponseWithUserApplicationLicense

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTileResponseWithUserApplicationLicense from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_application_tile_response_with_user_application_license_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTileResponseWithUserApplicationLicense.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTileResponseWithUserApplicationLicense.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_application_tile_response_with_user_application_license_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_application_tile_response_with_user_application_license_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTileResponseWithUserApplicationLicense from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_application_tile_response_with_user_application_license_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsResponsesApplicationTileResponseWithUserApplicationLicense.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_responses_application_tile_response_with_user_application_license_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


