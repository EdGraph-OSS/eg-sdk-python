# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**subscription_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**application_name** | **str** |  | [optional] 
**application_roles** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesRole]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesRole.md) |  | [optional] 
**start_date_time** | **str** |  | [optional] 
**end_date_time** | **str** |  | [optional] 
**actual_end_date_time** | **str** |  | [optional] 
**grace_period** | **int** |  | [optional] 
**number_of_licenses** | **int** |  | [optional] 
**assigned_licenses** | **int** |  | [optional] 
**max_assigned_licenses** | **int** |  | [optional] 
**last_max_assigned_licenses_date_time** | **str** |  | [optional] 
**license_type** | [**TenantApiTenantV1LicenseType**](TenantApiTenantV1LicenseType.md) |  | [optional] 
**subscription_status** | [**TenantApiTenantV1SubscriptionStatus**](TenantApiTenantV1SubscriptionStatus.md) |  | [optional] 
**auto_assign** | **bool** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_subscription_list_response_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_subscription_list_response_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_subscription_list_response_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_subscription_list_response_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_subscription_list_response_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesSubscriptionListResponseDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_subscription_list_response_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


