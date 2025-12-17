# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**latest_run** | [**EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsLatestRunDto**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsLatestRunDto.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_jobs_job_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_jobs_job_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_jobs_job_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_jobs_job_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_jobs_job_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsResponsesValidationResultsApiJobsJobDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_responses_validation_results_api_jobs_job_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


