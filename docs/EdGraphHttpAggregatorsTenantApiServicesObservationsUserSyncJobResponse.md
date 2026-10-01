# EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**mode** | [**DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobMode**](DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobMode.md) |  | [optional] 
**provider** | [**DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProvider**](DataSyncApiEdFiRosterSyncV1EdFiRosterSyncJobProvider.md) |  | [optional] 
**connection_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_secret** | **str** |  | [optional] 
**base_url** | **str** |  | [optional] 
**authentication_url** | **str** |  | [optional] 
**resources_url** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**ed_fi_instance_id** | **str** |  | [optional] 
**use_ssa_instead_of_seoaa** | [**DataSyncApiEdFiRosterSyncV1UseSSAInsteadOfSEOAAOptions**](DataSyncApiEdFiRosterSyncV1UseSSAInsteadOfSEOAAOptions.md) |  | [optional] 
**import_section_and_course_data** | **bool** |  | [optional] 
**use_staff_ed_org_contact_association_for_emails** | **bool** |  | [optional] 
**ignore_end_dates** | **bool** |  | [optional] 
**executions_list** | [**List[DataSyncApiJobExecutionV1JobExecutionListResponse]**](DataSyncApiJobExecutionV1JobExecutionListResponse.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_user_sync_job_response import EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_user_sync_job_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_user_sync_job_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_user_sync_job_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_user_sync_job_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsUserSyncJobResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_user_sync_job_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


