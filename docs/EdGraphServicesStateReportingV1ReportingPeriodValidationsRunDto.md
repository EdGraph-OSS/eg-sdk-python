# EdGraphServicesStateReportingV1ReportingPeriodValidationsRunDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**requested_date_time** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**queued_date_time** | **str** |  | [optional] 
**start_date_time** | **str** |  | [optional] 
**end_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_reporting_period_validations_run_dto import EdGraphServicesStateReportingV1ReportingPeriodValidationsRunDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodValidationsRunDto from a JSON string
ed_graph_services_state_reporting_v1_reporting_period_validations_run_dto_instance = EdGraphServicesStateReportingV1ReportingPeriodValidationsRunDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1ReportingPeriodValidationsRunDto.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_reporting_period_validations_run_dto_dict = ed_graph_services_state_reporting_v1_reporting_period_validations_run_dto_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1ReportingPeriodValidationsRunDto from a dict
ed_graph_services_state_reporting_v1_reporting_period_validations_run_dto_from_dict = EdGraphServicesStateReportingV1ReportingPeriodValidationsRunDto.from_dict(ed_graph_services_state_reporting_v1_reporting_period_validations_run_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


