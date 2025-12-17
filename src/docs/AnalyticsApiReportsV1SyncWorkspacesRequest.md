# AnalyticsApiReportsV1SyncWorkspacesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**configuration_id** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**reset_instance** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.analytics_api_reports_v1_sync_workspaces_request import AnalyticsApiReportsV1SyncWorkspacesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AnalyticsApiReportsV1SyncWorkspacesRequest from a JSON string
analytics_api_reports_v1_sync_workspaces_request_instance = AnalyticsApiReportsV1SyncWorkspacesRequest.from_json(json)
# print the JSON string representation of the object
print(AnalyticsApiReportsV1SyncWorkspacesRequest.to_json())

# convert the object into a dict
analytics_api_reports_v1_sync_workspaces_request_dict = analytics_api_reports_v1_sync_workspaces_request_instance.to_dict()
# create an instance of AnalyticsApiReportsV1SyncWorkspacesRequest from a dict
analytics_api_reports_v1_sync_workspaces_request_from_dict = AnalyticsApiReportsV1SyncWorkspacesRequest.from_dict(analytics_api_reports_v1_sync_workspaces_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


