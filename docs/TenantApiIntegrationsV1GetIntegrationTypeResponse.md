# TenantApiIntegrationsV1GetIntegrationTypeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**integration_type** | [**TenantApiIntegrationsV1IntegrationType**](TenantApiIntegrationsV1IntegrationType.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_get_integration_type_response import TenantApiIntegrationsV1GetIntegrationTypeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1GetIntegrationTypeResponse from a JSON string
tenant_api_integrations_v1_get_integration_type_response_instance = TenantApiIntegrationsV1GetIntegrationTypeResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1GetIntegrationTypeResponse.to_json())

# convert the object into a dict
tenant_api_integrations_v1_get_integration_type_response_dict = tenant_api_integrations_v1_get_integration_type_response_instance.to_dict()
# create an instance of TenantApiIntegrationsV1GetIntegrationTypeResponse from a dict
tenant_api_integrations_v1_get_integration_type_response_from_dict = TenantApiIntegrationsV1GetIntegrationTypeResponse.from_dict(tenant_api_integrations_v1_get_integration_type_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


