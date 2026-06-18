# TenantApiIntegrationsV1CreateIntegrationProductRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**integration_type_id** | **str** |  | [optional] 
**integration_vendor_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_create_integration_product_request import TenantApiIntegrationsV1CreateIntegrationProductRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1CreateIntegrationProductRequest from a JSON string
tenant_api_integrations_v1_create_integration_product_request_instance = TenantApiIntegrationsV1CreateIntegrationProductRequest.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1CreateIntegrationProductRequest.to_json())

# convert the object into a dict
tenant_api_integrations_v1_create_integration_product_request_dict = tenant_api_integrations_v1_create_integration_product_request_instance.to_dict()
# create an instance of TenantApiIntegrationsV1CreateIntegrationProductRequest from a dict
tenant_api_integrations_v1_create_integration_product_request_from_dict = TenantApiIntegrationsV1CreateIntegrationProductRequest.from_dict(tenant_api_integrations_v1_create_integration_product_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


