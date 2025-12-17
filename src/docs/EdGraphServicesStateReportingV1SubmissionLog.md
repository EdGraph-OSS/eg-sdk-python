# EdGraphServicesStateReportingV1SubmissionLog


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pipeline_execution_id** | **str** |  | [optional] 
**pipeline_execution_id_computed** | **str** |  | [optional] 
**run_id** | **str** |  | [optional] 
**operation_type** | **str** |  | [optional] 
**request_payload** | **str** |  | [optional] 
**request_url** | **str** |  | [optional] 
**resource** | **str** |  | [optional] 
**entity_name** | **str** |  | [optional] 
**response_headers** | **str** |  | [optional] 
**response_status_code** | **str** |  | [optional] 
**response_text** | **str** |  | [optional] 
**run_date_time** | **str** |  | [optional] 
**start_time** | **str** |  | [optional] 
**end_time** | **str** |  | [optional] 
**record_id** | **str** |  | [optional] 
**lake_id** | **str** |  | [optional] 
**ed_fi_location** | **str** |  | [optional] 
**ed_fi** | **str** |  | [optional] 
**ed_fi_id_modified** | **str** |  | [optional] 
**sap_pipeline** | **str** |  | [optional] 
**sap_pipeline_type** | **str** |  | [optional] 
**stage1_source_url** | **str** |  | [optional] 
**natural_key_hash** | **str** |  | [optional] 
**is_post_success** | **bool** |  | [optional] 
**run_date** | **str** |  | [optional] 
**entity_type** | **str** |  | [optional] 
**entity_name_computed** | **str** |  | [optional] 
**log_type** | **str** |  | [optional] 
**school_year** | **str** |  | [optional] 
**district_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_submission_log import EdGraphServicesStateReportingV1SubmissionLog

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SubmissionLog from a JSON string
ed_graph_services_state_reporting_v1_submission_log_instance = EdGraphServicesStateReportingV1SubmissionLog.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SubmissionLog.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_submission_log_dict = ed_graph_services_state_reporting_v1_submission_log_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SubmissionLog from a dict
ed_graph_services_state_reporting_v1_submission_log_from_dict = EdGraphServicesStateReportingV1SubmissionLog.from_dict(ed_graph_services_state_reporting_v1_submission_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


