# EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicense


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application_id** | **str** |  | [optional] 
**application_name** | **str** |  | [optional] 
**role** | [**EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicenseRole**](EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicenseRole.md) |  | [optional] 
**license_status** | **str** |  | [optional] 
**license_source** | **str** |  | [optional] 
**education_organization_id** | **int** |  | [optional] 
**education_organization_source** | **str** |  | [optional] 
**staff_classification** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license import EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicense

# TODO update the JSON string below
json = "{}"
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicense from a JSON string
ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_instance = EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicense.from_json(json)
# print the JSON string representation of the object
print(EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicense.to_json())

# convert the object into a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_dict = ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_instance.to_dict()
# create an instance of EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicense from a dict
ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_from_dict = EdGraphHttpAggregatorsTenantApiControllersV2ResponsesUserLicense.from_dict(ed_graph_http_aggregators_tenant_api_controllers_v2_responses_user_license_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


