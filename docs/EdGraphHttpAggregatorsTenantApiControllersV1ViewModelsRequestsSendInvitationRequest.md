# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**role** | **str** |  | [optional] 
**assign_license_requests** | [**List[EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseRequest]**](EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsLicensesAssignLicenseRequest.md) |  | [optional] 
**inviting_user_display_name** | **str** |  | [optional] 
**dont_send_email** | **bool** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsSendInvitationRequest.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_send_invitation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


