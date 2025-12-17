# ValidationsApiJobsV1ChildJob


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_id** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**child_job_id** | **str** |  | [optional] 
**child_job_name** | **str** |  | [optional] 
**job_execution_status** | [**ValidationsApiJobsV1JobExecutionStatus**](ValidationsApiJobsV1JobExecutionStatus.md) |  | [optional] 
**job_execution_start_date_time** | **str** |  | [optional] 
**job_execution_end_date_time** | **str** |  | [optional] 
**metrics** | [**List[ValidationsApiJobsV1Metric]**](ValidationsApiJobsV1Metric.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_jobs_v1_child_job import ValidationsApiJobsV1ChildJob

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiJobsV1ChildJob from a JSON string
validations_api_jobs_v1_child_job_instance = ValidationsApiJobsV1ChildJob.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiJobsV1ChildJob.to_json())

# convert the object into a dict
validations_api_jobs_v1_child_job_dict = validations_api_jobs_v1_child_job_instance.to_dict()
# create an instance of ValidationsApiJobsV1ChildJob from a dict
validations_api_jobs_v1_child_job_from_dict = ValidationsApiJobsV1ChildJob.from_dict(validations_api_jobs_v1_child_job_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


