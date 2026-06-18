# TenantApiIntegrationsV1IntegrationType


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_integration_type import TenantApiIntegrationsV1IntegrationType

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1IntegrationType from a JSON string
tenant_api_integrations_v1_integration_type_instance = TenantApiIntegrationsV1IntegrationType.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1IntegrationType.to_json())

# convert the object into a dict
tenant_api_integrations_v1_integration_type_dict = tenant_api_integrations_v1_integration_type_instance.to_dict()
# create an instance of TenantApiIntegrationsV1IntegrationType from a dict
tenant_api_integrations_v1_integration_type_from_dict = TenantApiIntegrationsV1IntegrationType.from_dict(tenant_api_integrations_v1_integration_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


