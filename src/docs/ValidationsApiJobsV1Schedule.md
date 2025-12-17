# ValidationsApiJobsV1Schedule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**begin_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**cron** | **str** |  | [optional] 
**time_zone** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_jobs_v1_schedule import ValidationsApiJobsV1Schedule

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiJobsV1Schedule from a JSON string
validations_api_jobs_v1_schedule_instance = ValidationsApiJobsV1Schedule.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiJobsV1Schedule.to_json())

# convert the object into a dict
validations_api_jobs_v1_schedule_dict = validations_api_jobs_v1_schedule_instance.to_dict()
# create an instance of ValidationsApiJobsV1Schedule from a dict
validations_api_jobs_v1_schedule_from_dict = ValidationsApiJobsV1Schedule.from_dict(validations_api_jobs_v1_schedule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


