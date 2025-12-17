# EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mode** | **str** |  | [optional] 
**use_ssa_instead_of_seoaa** | [**DataSyncApiEdFiRosterSyncV1UseSSAInsteadOfSEOAAOptions**](DataSyncApiEdFiRosterSyncV1UseSSAInsteadOfSEOAAOptions.md) |  | [optional] 
**import_section_and_course_data** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto import EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto from a JSON string
ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto_instance = EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto_dict = ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto from a dict
ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto_from_dict = EdGraphHttpAggregatorsTenantApiServicesEdFiRosterSyncCreateEdFiRosterSyncJobRequestDto.from_dict(ed_graph_http_aggregators_tenant_api_services_ed_fi_roster_sync_create_ed_fi_roster_sync_job_request_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


