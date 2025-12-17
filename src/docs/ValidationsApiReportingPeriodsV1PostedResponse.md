# ValidationsApiReportingPeriodsV1PostedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_posted_response import ValidationsApiReportingPeriodsV1PostedResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1PostedResponse from a JSON string
validations_api_reporting_periods_v1_posted_response_instance = ValidationsApiReportingPeriodsV1PostedResponse.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1PostedResponse.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_posted_response_dict = validations_api_reporting_periods_v1_posted_response_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1PostedResponse from a dict
validations_api_reporting_periods_v1_posted_response_from_dict = ValidationsApiReportingPeriodsV1PostedResponse.from_dict(validations_api_reporting_periods_v1_posted_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


