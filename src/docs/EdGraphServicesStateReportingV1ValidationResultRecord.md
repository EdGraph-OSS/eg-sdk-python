# EdGraphServicesStateReportingV1ValidationResultRecord


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**db_environment_id** | **str** |  | [optional] 
**collection_id** | **str** |  | [optional] 
**container_id** | **str** |  | [optional] 
**rule_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**run_id** | **str** |  | [optional] 
**exclude_from_post** | **bool** |  | [optional] 
**details** | **str** |  | [optional] 
**details_schema** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_validation_result_record import EdGraphServicesStateReportingV1ValidationResultRecord

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ValidationResultRecord from a JSON string
ed_graph_services_state_reporting_v1_validation_result_record_instance = EdGraphServicesStateReportingV1ValidationResultRecord.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ValidationResultRecord.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_validation_result_record_dict = ed_graph_services_state_reporting_v1_validation_result_record_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ValidationResultRecord from a dict
ed_graph_services_state_reporting_v1_validation_result_record_from_dict = EdGraphServicesStateReportingV1ValidationResultRecord.from_dict(ed_graph_services_state_reporting_v1_validation_result_record_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


