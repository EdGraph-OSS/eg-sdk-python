# EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolRequestDto

The body of a full school replace by id (not keyed on ExternalDataSourceSchoolId).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** | Must match the id in the route. | [optional] 
**tenant_id** | **UUID** | Must match the tenant in the route. | [optional] 
**external_data_source_school_id** | **str** |  | [optional] 
**school_state_short_code** | **str** | Required. | [optional] 
**school_name** | **str** | Required. | [optional] 
**district_state_short_code** | **str** |  | [optional] 
**school_state_long_code** | **str** |  | [optional] 
**school_local_code** | **str** |  | [optional] 
**district_local_code** | **str** |  | [optional] 
**district_state_code** | **str** |  | [optional] 
**district_name** | **str** |  | [optional] 
**grades_served** | **List[str]** |  | [optional] 
**address** | **str** |  | [optional] 
**lat** | **float** |  | [optional] 
**lon** | **float** |  | [optional] 
**phone** | **str** |  | [optional] 
**address_state_abbreviation** | **str** | Two-letter US state code, e.g. &#x60;TX&#x60;. Required when AddressState is sent. | [optional] 
**address_state** | **str** | Full name of the state in AddressStateAbbreviation, e.g. &#x60;Texas&#x60;. | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_request_dto import EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolRequestDto

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolRequestDto from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_request_dto_instance = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolRequestDto.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolRequestDto.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_request_dto_dict = ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_request_dto_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolRequestDto from a dict
ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_request_dto_from_dict = EdGraphHttpAggregatorsTenantApiControllersV1ViewModelsRequestsEnrollmentAdminUpdateSchoolRequestDto.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v1_view_models_requests_enrollment_admin_update_school_request_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


