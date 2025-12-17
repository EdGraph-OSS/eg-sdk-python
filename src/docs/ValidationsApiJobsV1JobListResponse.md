# ValidationsApiJobsV1JobListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**job_type_id** | **str** |  | [optional] 
**job_type_name** | **str** |  | [optional] 
**source_connection_id** | **str** |  | [optional] 
**destination_connection_id** | **str** |  | [optional] 
**profile_id** | **str** |  | [optional] 
**application_id** | **str** |  | [optional] 
**schedule** | [**ValidationsApiJobsV1Schedule**](ValidationsApiJobsV1Schedule.md) |  | [optional] 
**job_status** | [**ValidationsApiJobsV1JobStatus**](ValidationsApiJobsV1JobStatus.md) |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**job_execution_status** | [**ValidationsApiJobsV1JobExecutionStatus**](ValidationsApiJobsV1JobExecutionStatus.md) |  | [optional] 
**job_execution_start_date_time** | **str** |  | [optional] 
**job_execution_end_date_time** | **str** |  | [optional] 
**metrics** | [**List[ValidationsApiJobsV1Metric]**](ValidationsApiJobsV1Metric.md) |  | [optional] [readonly] 
**child_jobs** | [**List[ValidationsApiJobsV1ChildJob]**](ValidationsApiJobsV1ChildJob.md) |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**collection_id** | **str** |  | [optional] 
**job_execution_queued_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_jobs_v1_job_list_response import ValidationsApiJobsV1JobListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiJobsV1JobListResponse from a JSON string
validations_api_jobs_v1_job_list_response_instance = ValidationsApiJobsV1JobListResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiJobsV1JobListResponse.to_json())

# convert the object into a dict
validations_api_jobs_v1_job_list_response_dict = validations_api_jobs_v1_job_list_response_instance.to_dict()
# create an instance of ValidationsApiJobsV1JobListResponse from a dict
validations_api_jobs_v1_job_list_response_from_dict = ValidationsApiJobsV1JobListResponse.from_dict(validations_api_jobs_v1_job_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


