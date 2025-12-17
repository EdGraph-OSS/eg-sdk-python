# AnalyticsApiReportsV1ReportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**embed_token** | [**AnalyticsApiReportsV1AnalyticsEmbedToken**](AnalyticsApiReportsV1AnalyticsEmbedToken.md) |  | [optional] 
**report** | [**AnalyticsApiReportsV1AnalyticsReport**](AnalyticsApiReportsV1AnalyticsReport.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_reports_v1_report_response import AnalyticsApiReportsV1ReportResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiReportsV1ReportResponse from a JSON string
analytics_api_reports_v1_report_response_instance = AnalyticsApiReportsV1ReportResponse.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiReportsV1ReportResponse.to_json())

# convert the object into a dict
analytics_api_reports_v1_report_response_dict = analytics_api_reports_v1_report_response_instance.to_dict()
# create an instance of AnalyticsApiReportsV1ReportResponse from a dict
analytics_api_reports_v1_report_response_from_dict = AnalyticsApiReportsV1ReportResponse.from_dict(analytics_api_reports_v1_report_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


