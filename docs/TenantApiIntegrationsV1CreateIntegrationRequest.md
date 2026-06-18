# TenantApiIntegrationsV1CreateIntegrationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**integration_type_id** | **str** |  | [optional] 
**integration_vendor_id** | **str** |  | [optional] 
**integration_product_id** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_request import TenantApiIntegrationsV1CreateIntegrationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1CreateIntegrationRequest from a JSON string
tenant_api_integrations_v1_create_integration_request_instance = TenantApiIntegrationsV1CreateIntegrationRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1CreateIntegrationRequest.to_json())

# convert the object into a dict
tenant_api_integrations_v1_create_integration_request_dict = tenant_api_integrations_v1_create_integration_request_instance.to_dict()
# create an instance of TenantApiIntegrationsV1CreateIntegrationRequest from a dict
tenant_api_integrations_v1_create_integration_request_from_dict = TenantApiIntegrationsV1CreateIntegrationRequest.from_dict(tenant_api_integrations_v1_create_integration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


