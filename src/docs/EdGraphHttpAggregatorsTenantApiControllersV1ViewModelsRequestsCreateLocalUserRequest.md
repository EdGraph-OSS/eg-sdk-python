# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateLocalUserRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**user_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**role** | **str** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**lockout_enabled** | **bool** |  | [optional] 
**password** | **str** |  | [optional] 
**auto_generated_password** | **bool** |  | [optional] 
**two_factor_enabled** | **bool** |  | [optional] 
**assign_license_requests** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseRequest]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseRequest.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_local_user_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateLocalUserRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateLocalUserRequest from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_local_user_request_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateLocalUserRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateLocalUserRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_local_user_request_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_local_user_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateLocalUserRequest from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_local_user_request_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsCreateLocalUserRequest.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_create_local_user_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


