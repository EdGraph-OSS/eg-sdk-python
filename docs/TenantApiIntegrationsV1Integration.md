# TenantApiIntegrationsV1Integration


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**integration_type_id** | **str** |  | [optional] 
**integration_vendor_id** | **str** |  | [optional] 
**integration_product_id** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**tenant_id** | **str** |  | [optional] 

## Example

```python
from edgraph_platform_client.models.tenant_api_integrations_v1_integration import TenantApiIntegrationsV1Integration

# TODO update the JSON string below
json = "{}"
# create an instance of TenantApiIntegrationsV1Integration from a JSON string
tenant_api_integrations_v1_integration_instance = TenantApiIntegrationsV1Integration.from_json(json)
# print the JSON string representation of the object
print(TenantApiIntegrationsV1Integration.to_json())

# convert the object into a dict
tenant_api_integrations_v1_integration_dict = tenant_api_integrations_v1_integration_instance.to_dict()
# create an instance of TenantApiIntegrationsV1Integration from a dict
tenant_api_integrations_v1_integration_from_dict = TenantApiIntegrationsV1Integration.from_dict(tenant_api_integrations_v1_integration_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


