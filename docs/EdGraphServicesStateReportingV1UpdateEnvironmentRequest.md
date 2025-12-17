# EdGraphServicesStateReportingV1UpdateEnvironmentRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**db_environment_id** | **str** |  | [optional] 
**ed_fi_instance_id** | **str** |  | [optional] 
**mode** | **str** |  | [optional] 
**workspace_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_update_environment_request import EdGraphServicesStateReportingV1UpdateEnvironmentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1UpdateEnvironmentRequest from a JSON string
ed_graph_services_state_reporting_v1_update_environment_request_instance = EdGraphServicesStateReportingV1UpdateEnvironmentRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1UpdateEnvironmentRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_update_environment_request_dict = ed_graph_services_state_reporting_v1_update_environment_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1UpdateEnvironmentRequest from a dict
ed_graph_services_state_reporting_v1_update_environment_request_from_dict = EdGraphServicesStateReportingV1UpdateEnvironmentRequest.from_dict(ed_graph_services_state_reporting_v1_update_environment_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


