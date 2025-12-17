# EdGraphServicesStateReportingV1SubCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**category_id** | **str** |  | [optional] 
**sub_category_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_sub_category import EdGraphServicesStateReportingV1SubCategory

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1SubCategory from a JSON string
ed_graph_services_state_reporting_v1_sub_category_instance = EdGraphServicesStateReportingV1SubCategory.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1SubCategory.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_sub_category_dict = ed_graph_services_state_reporting_v1_sub_category_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1SubCategory from a dict
ed_graph_services_state_reporting_v1_sub_category_from_dict = EdGraphServicesStateReportingV1SubCategory.from_dict(ed_graph_services_state_reporting_v1_sub_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


