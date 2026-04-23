# EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**dashboard_id** | **str** |  | [optional] 
**preferences** | [**List[EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertReportPreferenceDetails]**](EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertReportPreferenceDetails.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request import EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request_dict = ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest from a dict
ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsUpsertDashboardPreferencesRequest.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_upsert_dashboard_preferences_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


