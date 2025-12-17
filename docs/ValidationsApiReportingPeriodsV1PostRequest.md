# ValidationsApiReportingPeriodsV1PostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**category_ids** | **List[str]** |  | [optional] [readonly] 
**school_year** | **int** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.validations_api_reporting_periods_v1_post_request import ValidationsApiReportingPeriodsV1PostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationsApiReportingPeriodsV1PostRequest from a JSON string
validations_api_reporting_periods_v1_post_request_instance = ValidationsApiReportingPeriodsV1PostRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationsApiReportingPeriodsV1PostRequest.to_json())

# convert the object into a dict
validations_api_reporting_periods_v1_post_request_dict = validations_api_reporting_periods_v1_post_request_instance.to_dict()
# create an instance of ValidationsApiReportingPeriodsV1PostRequest from a dict
validations_api_reporting_periods_v1_post_request_from_dict = ValidationsApiReportingPeriodsV1PostRequest.from_dict(validations_api_reporting_periods_v1_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


