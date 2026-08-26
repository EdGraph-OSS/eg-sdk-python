# EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsRequestsReportAccessRequest

Payload for setting a report's audience targeting. EdGraph.Platform.HttpAggregators.Tenant.Api.Controllers.v1.ViewModels.Requests.ReportAccessRequest.TargetAudience is one of  \"AnyoneInTenant\", \"UsersWithRoleInTenant\", or \"SpecificUsersInTenant\".

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**target_audience** | **str** |  | [optional] 
**staff_classifications** | **List[str]** | Targeted EdFi staff classifications (&#x60;namespace#codeValue&#x60;). | [optional] 
**users** | **List[str]** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_requests_report_access_request import EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsRequestsReportAccessRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsRequestsReportAccessRequest from a JSON string
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_requests_report_access_request_instance = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsRequestsReportAccessRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsRequestsReportAccessRequest.to_json())

# convert the object into a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_requests_report_access_request_dict = ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_requests_report_access_request_instance.to_dict()
# create an instance of EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsRequestsReportAccessRequest from a dict
ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_requests_report_access_request_from_dict = EdGraphPlatformHttpAggregatorsTenantApiControllersV1ViewModelsRequestsReportAccessRequest.from_dict(ed_graph_platform_http_aggregators_tenant_api_controllers_v1_view_models_requests_report_access_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


