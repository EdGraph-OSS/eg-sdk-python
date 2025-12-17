# EdGraphServicesStateReportingV1EnvironmentListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 
**db_environment_id** | **str** |  | [optional] 
**ed_fi_instance_id** | **str** |  | [optional] 
**mode** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_environment_list_response import EdGraphServicesStateReportingV1EnvironmentListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1EnvironmentListResponse from a JSON string
ed_graph_services_state_reporting_v1_environment_list_response_instance = EdGraphServicesStateReportingV1EnvironmentListResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1EnvironmentListResponse.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_environment_list_response_dict = ed_graph_services_state_reporting_v1_environment_list_response_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1EnvironmentListResponse from a dict
ed_graph_services_state_reporting_v1_environment_list_response_from_dict = EdGraphServicesStateReportingV1EnvironmentListResponse.from_dict(ed_graph_services_state_reporting_v1_environment_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


