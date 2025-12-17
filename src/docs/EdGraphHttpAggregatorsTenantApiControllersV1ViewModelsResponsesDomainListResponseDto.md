# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**domain_name** | **str** |  | [optional] 
**domain_status** | [**TenantApiTenantV1DomainStatus**](TenantApiTenantV1DomainStatus.md) |  | [optional] 
**auto_assign_users** | **bool** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**manually_verified** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_domain_list_response_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_domain_list_response_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_domain_list_response_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_domain_list_response_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_domain_list_response_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesDomainListResponseDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_domain_list_response_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


