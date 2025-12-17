# ValidationsApiReportingPeriodsV1ReportingPeriodDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**updated_by** | **str** |  | [optional] 
**deleted_at** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**tag_id** | **str** |  | [optional] 
**rule_ids** | **List[str]** |  | [optional] [readonly] 
**code** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**start_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**close_date** | **str** |  | [optional] 
**re_submission_date** | **str** |  | [optional] 
**auto_run_nightly** | **bool** |  | [optional] 
**selected** | **bool** |  | [optional] 
**last_run** | [**ValidationsApiReportingPeriodsV1ReportingPeriodValidationsRunDto**](ValidationsApiReportingPeriodsV1ReportingPeriodValidationsRunDto.md) |  | [optional] 
**latest_submission_request_date** | **str** |  | [optional] 
**latest_submission_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_reporting_period_dto import ValidationsApiReportingPeriodsV1ReportingPeriodDto

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1ReportingPeriodDto from a JSON string
validations_api_reporting_periods_v1_reporting_period_dto_instance = ValidationsApiReportingPeriodsV1ReportingPeriodDto.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1ReportingPeriodDto.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_reporting_period_dto_dict = validations_api_reporting_periods_v1_reporting_period_dto_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1ReportingPeriodDto from a dict
validations_api_reporting_periods_v1_reporting_period_dto_from_dict = ValidationsApiReportingPeriodsV1ReportingPeriodDto.from_dict(validations_api_reporting_periods_v1_reporting_period_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


