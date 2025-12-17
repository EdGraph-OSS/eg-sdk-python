# EdGraphServicesStateReportingV1PipelineRun


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**run_id** | **str** |  | [optional] 
**run_start** | **str** |  | [optional] 
**run_end** | **str** |  | [optional] 
**duration_in_ms** | **int** |  | [optional] 
**status** | **str** |  | [optional] 
**message** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_pipeline_run import EdGraphServicesStateReportingV1PipelineRun

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1PipelineRun from a JSON string
ed_graph_services_state_reporting_v1_pipeline_run_instance = EdGraphServicesStateReportingV1PipelineRun.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1PipelineRun.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_pipeline_run_dict = ed_graph_services_state_reporting_v1_pipeline_run_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1PipelineRun from a dict
ed_graph_services_state_reporting_v1_pipeline_run_from_dict = EdGraphServicesStateReportingV1PipelineRun.from_dict(ed_graph_services_state_reporting_v1_pipeline_run_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


