# AnalyticsApiReportsV1AnalyticsReport

Entities

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**report_id** | **str** |  | [optional] 
**group_id** | **str** |  | [optional] 
**dataset_ids** | [**List[AnalyticsApiReportsV1AnalyticsReportDataset]**](AnalyticsApiReportsV1AnalyticsReportDataset.md) |  | [optional] [readonly] 
**name** | **str** |  | [optional] 
**report_name** | **str** |  | [optional] 
**short_description** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**embed_url** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**source** | [**AnalyticsApiReportsV1ReportSource**](AnalyticsApiReportsV1ReportSource.md) |  | [optional] 
**is_visible** | **bool** |  | [optional] 
**tags** | **List[str]** |  | [optional] [readonly] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**last_uploaded_by** | **str** |  | [optional] 
**last_uploaded_date_time** | **str** |  | [optional] 
**download_uri** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**roles_required** | **bool** |  | [optional] 
**identity_required** | **bool** |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_reports_v1_analytics_report import AnalyticsApiReportsV1AnalyticsReport

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiReportsV1AnalyticsReport from a JSON string
analytics_api_reports_v1_analytics_report_instance = AnalyticsApiReportsV1AnalyticsReport.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiReportsV1AnalyticsReport.to_json())

# convert the object into a dict
analytics_api_reports_v1_analytics_report_dict = analytics_api_reports_v1_analytics_report_instance.to_dict()
# create an instance of AnalyticsApiReportsV1AnalyticsReport from a dict
analytics_api_reports_v1_analytics_report_from_dict = AnalyticsApiReportsV1AnalyticsReport.from_dict(analytics_api_reports_v1_analytics_report_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


