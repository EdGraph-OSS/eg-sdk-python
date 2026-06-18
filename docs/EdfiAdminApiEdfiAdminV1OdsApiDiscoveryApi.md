# EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **str** |  | [optional] 
**informational_version** | **str** |  | [optional] 
**suite** | **str** |  | [optional] 
**build** | **str** |  | [optional] 
**data_models** | [**List[EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApiDataModel]**](EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApiDataModel.md) |  | [optional] [readonly] 

## Example

```python
from edgraph_platform_client.models.edfi_admin_api_edfi_admin_v1_ods_api_discovery_api import EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi

# TODO update the JSON string below
json = "{}"
# create an instance of EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi from a JSON string
edfi_admin_api_edfi_admin_v1_ods_api_discovery_api_instance = EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi.from_json(json)
# print the JSON string representation of the object
print(EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi.to_json())

# convert the object into a dict
edfi_admin_api_edfi_admin_v1_ods_api_discovery_api_dict = edfi_admin_api_edfi_admin_v1_ods_api_discovery_api_instance.to_dict()
# create an instance of EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi from a dict
edfi_admin_api_edfi_admin_v1_ods_api_discovery_api_from_dict = EdfiAdminApiEdfiAdminV1OdsApiDiscoveryApi.from_dict(edfi_admin_api_edfi_admin_v1_ods_api_discovery_api_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


