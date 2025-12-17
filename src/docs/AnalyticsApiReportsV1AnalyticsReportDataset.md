# AnalyticsApiReportsV1AnalyticsReportDataset


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dataset_id** | **str** |  | [optional] 
**is_effective_identity_required** | **bool** |  | [optional] 
**is_effective_identity_roles_required** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_reports_v1_analytics_report_dataset import AnalyticsApiReportsV1AnalyticsReportDataset

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiReportsV1AnalyticsReportDataset from a JSON string
analytics_api_reports_v1_analytics_report_dataset_instance = AnalyticsApiReportsV1AnalyticsReportDataset.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiReportsV1AnalyticsReportDataset.to_json())

# convert the object into a dict
analytics_api_reports_v1_analytics_report_dataset_dict = analytics_api_reports_v1_analytics_report_dataset_instance.to_dict()
# create an instance of AnalyticsApiReportsV1AnalyticsReportDataset from a dict
analytics_api_reports_v1_analytics_report_dataset_from_dict = AnalyticsApiReportsV1AnalyticsReportDataset.from_dict(analytics_api_reports_v1_analytics_report_dataset_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


