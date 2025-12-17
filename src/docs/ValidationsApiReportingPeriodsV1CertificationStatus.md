# ValidationsApiReportingPeriodsV1CertificationStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period** | [**ValidationsApiReportingPeriodsV1ReportingPeriodDto**](ValidationsApiReportingPeriodsV1ReportingPeriodDto.md) |  | [optional] 
**certification_percentage** | **float** |  | [optional] 
**categories** | [**List[ValidationsApiReportingPeriodsV1CertificationStatusCategory]**](ValidationsApiReportingPeriodsV1CertificationStatusCategory.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_certification_status import ValidationsApiReportingPeriodsV1CertificationStatus

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1CertificationStatus from a JSON string
validations_api_reporting_periods_v1_certification_status_instance = ValidationsApiReportingPeriodsV1CertificationStatus.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1CertificationStatus.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_certification_status_dict = validations_api_reporting_periods_v1_certification_status_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1CertificationStatus from a dict
validations_api_reporting_periods_v1_certification_status_from_dict = ValidationsApiReportingPeriodsV1CertificationStatus.from_dict(validations_api_reporting_periods_v1_certification_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


