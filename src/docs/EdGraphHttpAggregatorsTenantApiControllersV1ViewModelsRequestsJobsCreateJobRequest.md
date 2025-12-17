# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**job_type_id** | **str** |  | [optional] 
**source_connection_id** | **str** |  | [optional] 
**destination_connection_id** | **str** |  | [optional] 
**profile_id** | **str** |  | [optional] 
**job_points** | **int** |  | [optional] 
**application_id** | **str** |  | [optional] 
**data_refresh_type** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsDataRefreshType**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsDataRefreshType.md) |  | [optional] 
**data_refresh_specific_date** | **str** |  | [optional] 
**max_api_failure** | **int** |  | [optional] 
**max_api_retry** | **int** |  | [optional] 
**job_complete_callback_url** | **str** |  | [optional] 
**job_metadata** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsJobMetadata]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsJobMetadata.md) |  | [optional] 
**schedule** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsSchedule**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsSchedule.md) |  | [optional] 
**notification_emails** | **List[str]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsCreateJobRequest.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_create_job_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


