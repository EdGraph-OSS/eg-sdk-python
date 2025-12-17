# ValidationsApiReportingPeriodsV1ReportingPeriodValidationsRunDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**requested_at** | **str** |  | [optional] 
**job_execution_id** | **str** |  | [optional] 
**job_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**queued_date_time** | **str** |  | [optional] 
**start_date_time** | **str** |  | [optional] 
**end_date_time** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_reporting_period_validations_run_dto import ValidationsApiReportingPeriodsV1ReportingPeriodValidationsRunDto

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1ReportingPeriodValidationsRunDto from a JSON string
validations_api_reporting_periods_v1_reporting_period_validations_run_dto_instance = ValidationsApiReportingPeriodsV1ReportingPeriodValidationsRunDto.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1ReportingPeriodValidationsRunDto.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_reporting_period_validations_run_dto_dict = validations_api_reporting_periods_v1_reporting_period_validations_run_dto_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1ReportingPeriodValidationsRunDto from a dict
validations_api_reporting_periods_v1_reporting_period_validations_run_dto_from_dict = ValidationsApiReportingPeriodsV1ReportingPeriodValidationsRunDto.from_dict(validations_api_reporting_periods_v1_reporting_period_validations_run_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


