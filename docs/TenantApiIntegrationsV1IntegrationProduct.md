# TenantApiIntegrationsV1IntegrationProduct


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**integration_type_id** | **str** |  | [optional] 
**integration_vendor_id** | **str** |  | [optional] 
**code** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_integration_product import TenantApiIntegrationsV1IntegrationProduct

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1IntegrationProduct from a JSON string
tenant_api_integrations_v1_integration_product_instance = TenantApiIntegrationsV1IntegrationProduct.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1IntegrationProduct.to_json())

# convert the object into a dict
tenant_api_integrations_v1_integration_product_dict = tenant_api_integrations_v1_integration_product_instance.to_dict()
# create an instance of TenantApiIntegrationsV1IntegrationProduct from a dict
tenant_api_integrations_v1_integration_product_from_dict = TenantApiIntegrationsV1IntegrationProduct.from_dict(tenant_api_integrations_v1_integration_product_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


