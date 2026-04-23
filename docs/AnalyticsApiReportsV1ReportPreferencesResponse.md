# AnalyticsApiReportsV1ReportPreferencesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**report_id** | **str** |  | [optional] 
**preferences** | [**List[AnalyticsApiReportsV1ReportPreferenceDetailsResponse]**](AnalyticsApiReportsV1ReportPreferenceDetailsResponse.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.analytics_api_reports_v1_report_preferences_response import AnalyticsApiReportsV1ReportPreferencesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiReportsV1ReportPreferencesResponse from a JSON string
analytics_api_reports_v1_report_preferences_response_instance = AnalyticsApiReportsV1ReportPreferencesResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiReportsV1ReportPreferencesResponse.to_json())

# convert the object into a dict
analytics_api_reports_v1_report_preferences_response_dict = analytics_api_reports_v1_report_preferences_response_instance.to_dict()
# create an instance of AnalyticsApiReportsV1ReportPreferencesResponse from a dict
analytics_api_reports_v1_report_preferences_response_from_dict = AnalyticsApiReportsV1ReportPreferencesResponse.from_dict(analytics_api_reports_v1_report_preferences_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


