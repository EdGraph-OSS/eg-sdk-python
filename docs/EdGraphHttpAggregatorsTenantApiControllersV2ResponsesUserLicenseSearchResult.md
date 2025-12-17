# EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicenseSearchResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_index** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 
**count** | **int** |  | [optional] 
**data** | [**List[EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicense]**](EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicense.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_search_result import EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicenseSearchResult

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicenseSearchResult from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_search_result_instance = EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicenseSearchResult.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicenseSearchResult.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_search_result_dict = ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_search_result_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicenseSearchResult from a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_search_result_from_dict = EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicenseSearchResult.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_search_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


