# EdGraphServicesStateReportingV1Category


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **str** |  | [optional] 
**environment_id** | **str** |  | [optional] 
**reporting_period_id** | **str** |  | [optional] 
**category_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**certification_status** | **str** |  | [optional] 
**data_owner** | [**EdGraphServicesStateReportingV1DataUser**](EdGraphServicesStateReportingV1DataUser.md) |  | [optional] 
**data_stewards** | [**List[EdGraphServicesStateReportingV1DataUser]**](EdGraphServicesStateReportingV1DataUser.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.ed_graph_services_state_reporting_v1_category import EdGraphServicesStateReportingV1Category

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphServicesStateReportingV1Category from a JSON string
ed_graph_services_state_reporting_v1_category_instance = EdGraphServicesStateReportingV1Category.from_json(json)
# print the JSON string representation of the object
print(EdGraphServicesStateReportingV1Category.to_json())

# convert the object into a dict
ed_graph_services_state_reporting_v1_category_dict = ed_graph_services_state_reporting_v1_category_instance.to_dict()
# create an instance of EdGraphServicesStateReportingV1Category from a dict
ed_graph_services_state_reporting_v1_category_from_dict = EdGraphServicesStateReportingV1Category.from_dict(ed_graph_services_state_reporting_v1_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


