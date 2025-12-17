# ValidationsApiReportingPeriodsV1UpdateBulkRequestTypesReportingPeriod


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reporting_period_id** | **str** |  | [optional] 
**start_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**re_submission_date** | **str** |  | [optional] 
**auto_run_nightly** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_update_bulk_request_types_reporting_period import ValidationsApiReportingPeriodsV1UpdateBulkRequestTypesReportingPeriod

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1UpdateBulkRequestTypesReportingPeriod from a JSON string
validations_api_reporting_periods_v1_update_bulk_request_types_reporting_period_instance = ValidationsApiReportingPeriodsV1UpdateBulkRequestTypesReportingPeriod.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1UpdateBulkRequestTypesReportingPeriod.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_update_bulk_request_types_reporting_period_dict = validations_api_reporting_periods_v1_update_bulk_request_types_reporting_period_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1UpdateBulkRequestTypesReportingPeriod from a dict
validations_api_reporting_periods_v1_update_bulk_request_types_reporting_period_from_dict = ValidationsApiReportingPeriodsV1UpdateBulkRequestTypesReportingPeriod.from_dict(validations_api_reporting_periods_v1_update_bulk_request_types_reporting_period_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


