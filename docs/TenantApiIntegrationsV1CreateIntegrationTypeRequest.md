# TenantApiIntegrationsV1CreateIntegrationTypeRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_type_request import TenantApiIntegrationsV1CreateIntegrationTypeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1CreateIntegrationTypeRequest from a JSON string
tenant_api_integrations_v1_create_integration_type_request_instance = TenantApiIntegrationsV1CreateIntegrationTypeRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1CreateIntegrationTypeRequest.to_json())

# convert the object into a dict
tenant_api_integrations_v1_create_integration_type_request_dict = tenant_api_integrations_v1_create_integration_type_request_instance.to_dict()
# create an instance of TenantApiIntegrationsV1CreateIntegrationTypeRequest from a dict
tenant_api_integrations_v1_create_integration_type_request_from_dict = TenantApiIntegrationsV1CreateIntegrationTypeRequest.from_dict(tenant_api_integrations_v1_create_integration_type_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


