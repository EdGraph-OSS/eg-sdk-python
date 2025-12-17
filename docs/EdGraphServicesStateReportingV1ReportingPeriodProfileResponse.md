# EdGraphServicesStateReportingV1ReportingPeriodProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**tag_id** | **str** |  | [optional] 
**steps** | [**List[EdGraphServicesStateReportingV1ReportingPeriodStep]**](EdGraphServicesStateReportingV1ReportingPeriodStep.md) |  | [optional] [readonly] 
**rule_ids** | **List[str]** |  | [optional] [readonly] 
**code** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**start_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**close_date** | **str** |  | [optional] 
**is_closed** | **bool** |  | [optional] 
**re_submission_date** | **str** |  | [optional] 
**auto_run_nightly** | **bool** |  | [optional] 
**selected** | **bool** |  | [optional] 
**last_run** | [**EdGraphServicesStateReportingV1ReportingPeriodValidationsRunDto**](EdGraphServicesStateReportingV1ReportingPeriodValidationsRunDto.md) |  | [optional] 
**latest_submission_request_date** | **str** |  | [optional] 
**latest_submission_id** | **str** |  | [optional] 
**current_step** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_profile_response import EdGraphServicesStateReportingV1ReportingPeriodProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodProfileResponse from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_profile_response_instance = EdGraphServicesStateReportingV1ReportingPeriodProfileResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodProfileResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_profile_response_dict = ed_graph_services_state_reporting_v1_reporting_period_profile_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodProfileResponse from a dict
ed_graph_services_state_reporting_v1_reporting_period_profile_response_from_dict = EdGraphServicesStateReportingV1ReportingPeriodProfileResponse.from_dict(ed_graph_services_state_reporting_v1_reporting_period_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


