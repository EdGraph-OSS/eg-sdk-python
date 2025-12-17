# EdGraphServicesStateReportingV1CreateEnvironmentRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**year** | **int** |  | [optional] 
**db_environment_id** | **str** |  | [optional] 
**ed_fi_instance_id** | **str** |  | [optional] 
**mode** | **str** |  | [optional] 
**workspace_name** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_create_environment_request import EdGraphServicesStateReportingV1CreateEnvironmentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1CreateEnvironmentRequest from a JSON string
ed_graph_services_state_reporting_v1_create_environment_request_instance = EdGraphServicesStateReportingV1CreateEnvironmentRequest.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1CreateEnvironmentRequest.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_create_environment_request_dict = ed_graph_services_state_reporting_v1_create_environment_request_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1CreateEnvironmentRequest from a dict
ed_graph_services_state_reporting_v1_create_environment_request_from_dict = EdGraphServicesStateReportingV1CreateEnvironmentRequest.from_dict(ed_graph_services_state_reporting_v1_create_environment_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


