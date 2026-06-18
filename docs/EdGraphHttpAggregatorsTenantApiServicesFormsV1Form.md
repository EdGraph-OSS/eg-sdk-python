# EdGraphHttpAggregatorsTenantApiServicesFormsV1Form


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **UUID** |  | [optional] 
**tenant_id** | **UUID** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**anonymous** | **bool** |  | [optional] 
**status** | **str** |  | [optional] 
**submission_count** | **int** |  | [optional] 
**created_by** | **str** |  | [optional] 
**created_date_time** | **str** |  | [optional] 
**last_modified_by** | **str** |  | [optional] 
**last_modified_date_time** | **str** |  | [optional] 
**deleted_by** | **str** |  | [optional] 
**deleted_date_time** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**image** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_forms_v1_form import EdGraphHttpAggregatorsTenantApiServicesFormsV1Form

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesFormsV1Form from a JSON string
ed_graph_http_aggregators_tenant_api_services_forms_v1_form_instance = EdGraphHttpAggregatorsTenantApiServicesFormsV1Form.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesFormsV1Form.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_forms_v1_form_dict = ed_graph_http_aggregators_tenant_api_services_forms_v1_form_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesFormsV1Form from a dict
ed_graph_http_aggregators_tenant_api_services_forms_v1_form_from_dict = EdGraphHttpAggregatorsTenantApiServicesFormsV1Form.from_dict(ed_graph_http_aggregators_tenant_api_services_forms_v1_form_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


