# ValidationsApiReportingPeriodsV1UpdatedBulkResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period_ids** | **List[str]** |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_updated_bulk_response import ValidationsApiReportingPeriodsV1UpdatedBulkResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1UpdatedBulkResponse from a JSON string
validations_api_reporting_periods_v1_updated_bulk_response_instance = ValidationsApiReportingPeriodsV1UpdatedBulkResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1UpdatedBulkResponse.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_updated_bulk_response_dict = validations_api_reporting_periods_v1_updated_bulk_response_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1UpdatedBulkResponse from a dict
validations_api_reporting_periods_v1_updated_bulk_response_from_dict = ValidationsApiReportingPeriodsV1UpdatedBulkResponse.from_dict(validations_api_reporting_periods_v1_updated_bulk_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


