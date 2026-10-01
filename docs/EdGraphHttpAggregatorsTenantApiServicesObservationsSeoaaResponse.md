# EdGraphHttpAggregatorsTenantApiServicesObservationsSeoaaResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**seoaa_id** | **str** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 
**name_of_institution** | **str** |  | [optional] 
**short_name_of_institution** | **str** |  | [optional] 
**staff_classification_descriptor** | **str** |  | [optional] 
**staff_unique_id** | **str** |  | [optional] 
**begin_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 
**source** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_services_observations_seoaa_response import EdGraphHttpAggregatorsTenantApiServicesObservationsSeoaaResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsSeoaaResponse from a JSON string
ed_graph_http_aggregators_tenant_api_services_observations_seoaa_response_instance = EdGraphHttpAggregatorsTenantApiServicesObservationsSeoaaResponse.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiServicesObservationsSeoaaResponse.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_services_observations_seoaa_response_dict = ed_graph_http_aggregators_tenant_api_services_observations_seoaa_response_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiServicesObservationsSeoaaResponse from a dict
ed_graph_http_aggregators_tenant_api_services_observations_seoaa_response_from_dict = EdGraphHttpAggregatorsTenantApiServicesObservationsSeoaaResponse.from_dict(ed_graph_http_aggregators_tenant_api_services_observations_seoaa_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


