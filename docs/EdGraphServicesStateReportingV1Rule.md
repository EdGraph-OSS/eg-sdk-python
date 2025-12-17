# EdGraphServicesStateReportingV1Rule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category_id** | **str** |  | [optional] 
**sub_category_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**rule_identification** | **str** |  | [optional] 
**error_severity_level** | **str** |  | [optional] 
**last_execution_total_results** | **int** |  | [optional] 
**last_execution_total_invalid_results** | **int** |  | [optional] 
**id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_rule import EdGraphServicesStateReportingV1Rule

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1Rule from a JSON string
ed_graph_services_state_reporting_v1_rule_instance = EdGraphServicesStateReportingV1Rule.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1Rule.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_rule_dict = ed_graph_services_state_reporting_v1_rule_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1Rule from a dict
ed_graph_services_state_reporting_v1_rule_from_dict = EdGraphServicesStateReportingV1Rule.from_dict(ed_graph_services_state_reporting_v1_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


