# EdGraphServicesStateReportingV1SubmissionProfile


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**updated_by** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**pipeline_run** | [**EdGraphServicesStateReportingV1PipelineRun**](EdGraphServicesStateReportingV1PipelineRun.md) |  | [optional] 
**status** | **str** |  | [optional] 
**pipeline_run_id** | **str** |  | [optional] 
**pipeline_run_details** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_profile import EdGraphServicesStateReportingV1SubmissionProfile

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SubmissionProfile from a JSON string
ed_graph_services_state_reporting_v1_submission_profile_instance = EdGraphServicesStateReportingV1SubmissionProfile.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SubmissionProfile.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_submission_profile_dict = ed_graph_services_state_reporting_v1_submission_profile_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SubmissionProfile from a dict
ed_graph_services_state_reporting_v1_submission_profile_from_dict = EdGraphServicesStateReportingV1SubmissionProfile.from_dict(ed_graph_services_state_reporting_v1_submission_profile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


