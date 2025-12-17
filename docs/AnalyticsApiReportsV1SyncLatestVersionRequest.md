# AnalyticsApiReportsV1SyncLatestVersionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**configuration_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**report_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_reports_v1_sync_latest_version_request import AnalyticsApiReportsV1SyncLatestVersionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiReportsV1SyncLatestVersionRequest from a JSON string
analytics_api_reports_v1_sync_latest_version_request_instance = AnalyticsApiReportsV1SyncLatestVersionRequest.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiReportsV1SyncLatestVersionRequest.to_json())

# convert the object into a dict
analytics_api_reports_v1_sync_latest_version_request_dict = analytics_api_reports_v1_sync_latest_version_request_instance.to_dict()
# create an instance of AnalyticsApiReportsV1SyncLatestVersionRequest from a dict
analytics_api_reports_v1_sync_latest_version_request_from_dict = AnalyticsApiReportsV1SyncLatestVersionRequest.from_dict(analytics_api_reports_v1_sync_latest_version_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


