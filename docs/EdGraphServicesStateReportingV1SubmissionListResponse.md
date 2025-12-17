# EdGraphServicesStateReportingV1SubmissionListResponse


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
**status** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_list_response import EdGraphServicesStateReportingV1SubmissionListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SubmissionListResponse from a JSON string
ed_graph_services_state_reporting_v1_submission_list_response_instance = EdGraphServicesStateReportingV1SubmissionListResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SubmissionListResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_submission_list_response_dict = ed_graph_services_state_reporting_v1_submission_list_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SubmissionListResponse from a dict
ed_graph_services_state_reporting_v1_submission_list_response_from_dict = EdGraphServicesStateReportingV1SubmissionListResponse.from_dict(ed_graph_services_state_reporting_v1_submission_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


