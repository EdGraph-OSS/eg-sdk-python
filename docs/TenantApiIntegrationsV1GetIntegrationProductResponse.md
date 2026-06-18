# TenantApiIntegrationsV1GetIntegrationProductResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**integration_product** | [**TenantApiIntegrationsV1IntegrationProduct**](TenantApiIntegrationsV1IntegrationProduct.md) |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_get_integration_product_response import TenantApiIntegrationsV1GetIntegrationProductResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1GetIntegrationProductResponse from a JSON string
tenant_api_integrations_v1_get_integration_product_response_instance = TenantApiIntegrationsV1GetIntegrationProductResponse.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1GetIntegrationProductResponse.to_json())

# convert the object into a dict
tenant_api_integrations_v1_get_integration_product_response_dict = tenant_api_integrations_v1_get_integration_product_response_instance.to_dict()
# create an instance of TenantApiIntegrationsV1GetIntegrationProductResponse from a dict
tenant_api_integrations_v1_get_integration_product_response_from_dict = TenantApiIntegrationsV1GetIntegrationProductResponse.from_dict(tenant_api_integrations_v1_get_integration_product_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


