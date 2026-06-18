# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**schedule** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsSchedule**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsSchedule.md) |  | [optional] 
**notification_emails** | **List[str]** |  | [optional] 
**categories** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsJobCategory]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsJobCategory.md) |  | [optional] 
**environment_id** | **UUID** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsJobsUpdateValidationJobRequest.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_jobs_update_validation_job_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


